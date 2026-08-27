function doPost(e) {
  try {
    // 1. เชื่อมต่อกับ Sheet ผ่าน ID ที่คุณส่งมา
    var sheetId = '1Jyb1oLHJfGHzxMg35E4qC-pNKgF1dCnLMKx1ngetpt0';
    var ss = SpreadsheetApp.openById(sheetId);
    
    // เลือก Sheet หน้าแรกที่ใช้งานอยู่ (หากตั้งชื่อเฉพาะไว้ให้เปลี่ยนเป็น ss.getSheetByName("ชื่อชีต"); )
    var sheet = ss.getActiveSheet(); 
    
    // 2. ดึงข้อมูลจากฟอร์ม (อ้างอิงชื่อจาก attribute 'name' ใน HTML)
    // ใส่ || '-' เพื่อป้องกันกรณีผู้ใช้ไม่ได้กรอกข้อมูลบางช่อง ข้อมูลจะได้ไม่รวน
    var name = e.parameter.name || '-';
    var interest = e.parameter.interest || '-';
    var date = e.parameter.date || '-';
    var time = e.parameter.time || '-';
    var note = e.parameter.note || '-';
    var timestamp = new Date(); 
    
    // 3. นำข้อมูลทั้งหมดไปต่อท้ายเป็นแถวใหม่ (เรียงคอลัมน์ให้ตรงกับที่ตั้งไว้)
    sheet.appendRow([timestamp, name, interest, date, time, note]);
    
    // 4. ส่งผลลัพธ์กลับไปยังฝั่งหน้าเว็บว่าสำเร็จ
    return ContentService
      .createTextOutput(JSON.stringify({ "result": "success", "row": sheet.getLastRow() }))
      .setMimeType(ContentService.MimeType.JSON);
      
  } catch (error) {
    // หากบันทึกไม่สำเร็จ ให้ส่งข้อความ Error กลับไป
    return ContentService
      .createTextOutput(JSON.stringify({ "result": "error", "message": error.toString() }))
      .setMimeType(ContentService.MimeType.JSON);
  }
}
