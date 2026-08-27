<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Natural IT Store - Web App</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;400;600&family=Sarabun:wght@400;600&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'nature-bg': '#F4F1EA',
                        'nature-card': '#FFFFFF',
                        'nature-green': '#557A46',
                        'nature-hover': '#3B572E',
                        'nature-brown': '#8D7B68',
                        'nature-text': '#2C3E2E',
                        'nature-light': '#737373',
                        'nature-border': '#E6E2D6',
                    },
                    fontFamily: {
                        sans: ['Sarabun', 'Prompt', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        * {
            -webkit-tap-highlight-color: transparent;
        }

        body {
            background-color: #F4F1EA;
        }

        .app-container {
            width: 100%;
            max-width: 480px; /* Mobile width */
            height: 100vh;
            margin: 0 auto;
            position: relative;
            display: flex;
            flex-direction: column;
            background-color: #F4F1EA;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
            overflow: hidden; /* Prevent body scroll, manage in main-content */
        }

        .main-content {
            flex: 1;
            overflow-y: auto;
            padding-bottom: 80px; /* Space for bottom nav */
        }

        /* Hide pages by default */
        .page {
            display: none;
            animation: fadeIn 0.3s ease-out forwards;
        }
        
        .page.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Modal Overlay */
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 100;
            justify-content: center;
            align-items: center;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .modal-overlay.show {
            display: flex;
            opacity: 1;
        }

        .modal-content {
            background-color: white;
            padding: 30px;
            border-radius: 12px;
            text-align: center;
            width: 80%;
            max-width: 300px;
            transform: scale(0.9);
            transition: transform 0.3s ease;
            border-top: 4px solid var(--primary-green);
        }

        .modal-overlay.show .modal-content {
            transform: scale(1);
        }
    </style>
</head>
<body class="text-nature-text antialiased">

    <div class="app-container bg-nature-bg">
        
        <!-- Header -->
        <header class="bg-nature-green text-white p-5 text-center text-xl font-semibold rounded-b-2xl shadow-md z-10">
            🍃 Natural IT Store
        </header>

        <!-- Main Content Area -->
        <div class="main-content p-5">
            
            <!-- Page 1: Home -->
            <div id="page-home" class="page active">
                
                <!-- Hero Banner -->
                <div class="bg-nature-card rounded-xl p-5 text-center mb-6 border border-nature-border shadow-sm">
                    <h3 class="text-nature-green text-lg font-semibold mb-2">ยินดีต้อนรับ</h3>
                    <p class="text-sm text-nature-light">จำหน่ายอุปกรณ์ IT และให้คำปรึกษาด้วยความเป็นกันเอง ภายใต้บรรยากาศสบายๆ</p>
                </div>
                
                <!-- Categories -->
                <h4 class="mb-4 text-nature-green font-semibold">หมวดหมู่บริการของเรา</h4>
                <div class="grid grid-cols-2 gap-4">
                    
                    <div class="bg-nature-card rounded-xl p-5 text-center border border-nature-border shadow-sm cursor-pointer transition transform active:scale-95" onclick="goToBooking('notebook')">
                        <div class="text-3xl mb-2">💻</div>
                        <div class="text-sm font-semibold text-nature-brown">โน้ตบุ๊ก / PC</div>
                    </div>
                    
                    <div class="bg-nature-card rounded-xl p-5 text-center border border-nature-border shadow-sm cursor-pointer transition transform active:scale-95" onclick="goToBooking('gadget')">
                        <div class="text-3xl mb-2">🎧</div>
                        <div class="text-sm font-semibold text-nature-brown">อุปกรณ์เสริม</div>
                    </div>
                    
                    <div class="bg-nature-card rounded-xl p-5 text-center border border-nature-border shadow-sm cursor-pointer transition transform active:scale-95" onclick="goToBooking('network')">
                        <div class="text-3xl mb-2">🌐</div>
                        <div class="text-sm font-semibold text-nature-brown">ระบบเครือข่าย</div>
                    </div>
                    
                    <div class="bg-nature-card rounded-xl p-5 text-center border border-nature-border shadow-sm cursor-pointer transition transform active:scale-95" onclick="goToBooking('consult')">
                        <div class="text-3xl mb-2">🛠️</div>
                        <div class="text-sm font-semibold text-nature-brown">จัดสเปค & ซ่อม</div>
                    </div>
                    
                </div>
            </div>

            <!-- Page 2: Booking -->
            <div id="page-booking" class="page">
                <div class="bg-nature-card p-6 rounded-xl border-t-4 border-nature-green shadow-md">
                    <h3 class="text-nature-green text-center font-semibold mb-6 text-lg">นัดหมายเข้ารับบริการ</h3>
                    
                    <form id="bookingForm" onsubmit="submitForm(event)">
                        
                        <div class="mb-4">
                            <label class="block mb-2 font-semibold text-sm text-nature-text">ชื่อ-นามสกุล</label>
                            <input type="text" name="name" placeholder="ระบุชื่อของคุณ" required
                                class="w-full p-3 border border-nature-border rounded-lg bg-gray-50 text-sm focus:outline-none focus:border-nature-green focus:ring-1 focus:ring-nature-green focus:bg-white transition-colors">
                        </div>
                        
                        <div class="mb-4">
                            <label class="block mb-2 font-semibold text-sm text-nature-text">ความสนใจ</label>
                            <select id="select-interest" name="interest" required
                                class="w-full p-3 border border-nature-border rounded-lg bg-gray-50 text-sm focus:outline-none focus:border-nature-green focus:ring-1 focus:ring-nature-green focus:bg-white transition-colors appearance-none">
                                <option value="" disabled selected>-- กรุณาเลือก --</option>
                                <option value="notebook">โน้ตบุ๊ก / PC</option>
                                <option value="gadget">อุปกรณ์เสริม (Mouse, หูฟัง)</option>
                                <option value="network">ระบบเครือข่าย</option>
                                <option value="consult">จัดสเปค / ส่งซ่อม</option>
                            </select>
                        </div>
                        
                        <div class="mb-4">
                            <label class="block mb-2 font-semibold text-sm text-nature-text">วันที่ต้องการเข้ามา</label>
                            <input type="date" name="date" required
                                class="w-full p-3 border border-nature-border rounded-lg bg-gray-50 text-sm focus:outline-none focus:border-nature-green focus:ring-1 focus:ring-nature-green focus:bg-white transition-colors">
                        </div>
                        
                        <div class="mb-4">
                            <label class="block mb-2 font-semibold text-sm text-nature-text">เวลา</label>
                            <input type="time" name="time" required
                                class="w-full p-3 border border-nature-border rounded-lg bg-gray-50 text-sm focus:outline-none focus:border-nature-green focus:ring-1 focus:ring-nature-green focus:bg-white transition-colors">
                        </div>
                        
                        <div class="mb-4">
                            <label class="block mb-2 font-semibold text-sm text-nature-text">รายละเอียดเพิ่มเติม</label>
                            <textarea name="note" rows="3" placeholder="ระบุรุ่น หรือ งบประมาณ"
                                class="w-full p-3 border border-nature-border rounded-lg bg-gray-50 text-sm focus:outline-none focus:border-nature-green focus:ring-1 focus:ring-nature-green focus:bg-white transition-colors"></textarea>
                        </div>
                        
                        <button type="submit" id="submitBtn" class="w-full py-3 bg-nature-green text-white rounded-lg font-semibold text-lg hover:bg-nature-hover transition-colors shadow-md active:scale-95 transform">
                            ยืนยันการนัดหมาย
                        </button>
                    </form>
                </div>
            </div>

        </div> <!-- End of main-content -->

        <!-- Bottom Navigation -->
        <nav class="absolute bottom-0 left-0 w-full bg-white flex justify-around py-2 border-t border-nature-border shadow-[0_-2px_10px_rgba(0,0,0,0.05)] z-20">
            
            <div class="nav-item active text-center text-nature-light cursor-pointer flex-1 py-1 transition-colors hover:text-nature-green" id="nav-home" onclick="switchPage('home')">
                <div class="text-xl mb-1">🏠</div>
                <div class="text-xs font-semibold">หน้าแรก</div>
            </div>
            
            <div class="nav-item text-center text-nature-light cursor-pointer flex-1 py-1 transition-colors hover:text-nature-green" id="nav-booking" onclick="switchPage('booking')">
                <div class="text-xl mb-1">📅</div>
                <div class="text-xs font-semibold">จองคิว</div>
            </div>
            
            <div class="nav-item text-center text-nature-light cursor-pointer flex-1 py-1 transition-colors hover:text-nature-green" id="nav-contact" onclick="showContactModal()">
                <div class="text-xl mb-1">💬</div>
                <div class="text-xs font-semibold">ติดต่อ</div>
            </div>
            
        </nav>
        
        <!-- Success Modal -->
        <div id="success-modal" class="modal-overlay">
            <div class="modal-content bg-white p-6 rounded-xl shadow-xl w-10/12 max-w-sm text-center border-t-4 border-nature-green">
                <div class="text-4xl mb-4">🌿</div>
                <h3 class="text-lg font-bold text-nature-green mb-2">สำเร็จ!</h3>
                <p class="text-sm text-nature-text mb-6">บันทึกการนัดหมายเรียบร้อยแล้ว<br>ทางร้านจะรอต้อนรับคุณครับ</p>
                <button onclick="closeModal('success-modal'); switchPage('home');" class="w-full py-2 px-4 bg-nature-green text-white rounded-lg font-semibold hover:bg-nature-hover transition-colors">
                    ตกลง
                </button>
            </div>
        </div>

        <!-- Contact Modal -->
        <div id="contact-modal" class="modal-overlay">
            <div class="modal-content bg-white p-6 rounded-xl shadow-xl w-10/12 max-w-sm text-center border-t-4 border-nature-green">
                <div class="text-4xl mb-4">💬</div>
                <h3 class="text-lg font-bold text-nature-green mb-2">ติดต่อเรา</h3>
                <p class="text-sm text-nature-text mb-6">Line: @NaturalIT<br>โทร: 080-123-4567<br>เวลาทำการ: 10:00 - 19:00 น.</p>
                <button onclick="closeModal('contact-modal')" class="w-full py-2 px-4 bg-nature-green text-white rounded-lg font-semibold hover:bg-nature-hover transition-colors">
                    ปิด
                </button>
            </div>
        </div>

    </div>

    <!-- JavaScript สำหรับควบคุม Web App -->
    <script>
        
        // แนบฟังก์ชันไปที่ window object เพื่อป้องกันปัญหามองไม่เห็นฟังก์ชันในสภาพแวดล้อมจำลอง (Sandbox/Iframe)
        window.switchPage = function(pageName) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            
            // Remove active class from all nav items
            document.querySelectorAll('.nav-item').forEach(nav => {
                nav.classList.remove('text-nature-green');
                nav.classList.add('text-nature-light');
            });

            // Show selected page
            document.getElementById('page-' + pageName).classList.add('active');
            
            // Highlight selected nav item
            const navElement = document.getElementById('nav-' + pageName);
            if (navElement) {
                navElement.classList.remove('text-nature-light');
                navElement.classList.add('text-nature-green');
            }
            
            // Scroll to top when switching pages
            document.querySelector('.main-content').scrollTop = 0;
        };

        function goToBooking(interestValue) {
            // สลับไปหน้า Booking
            switchPage('booking');
            // เซ็ตค่า Dropdown ตามหมวดหมู่ที่คลิกจากหน้าแรก
            document.getElementById('select-interest').value = interestValue;
        }

        // URL ที่ได้จาก Google Apps Script
        const scriptURL = 'https://script.google.com/macros/s/AKfycbzL6hoFP_vEKgvJMJFEoswlX8qlAazl-A7S4z6Qj6GiGT693pENd9pJbYdF895nIHJlAQ/exec';

        function submitForm(event) {
            event.preventDefault(); // ป้องกันการรีเฟรชหน้า
            
            const form = event.target;
            const submitBtn = document.getElementById('submitBtn');
            const originalBtnText = submitBtn.innerText;
            
            // เปลี่ยนข้อความปุ่มเพื่อแสดงว่ากำลังส่งข้อมูล และกันไม่ให้กดซ้ำ
            submitBtn.innerText = 'กำลังบันทึกข้อมูล...';
            submitBtn.disabled = true;
            submitBtn.style.opacity = '0.7';

            // ส่งข้อมูลไปยัง Google Apps Script
            fetch(scriptURL, { method: 'POST', body: new FormData(form)})
                .then(response => {
                    // ล้างฟอร์ม
                    form.reset();
                    // แสดง Modal แจ้งเตือน
                    window.showModal('success-modal');
                })
                .catch(error => {
                    console.error('Error!', error.message);
                    // ป้องกัน Error ระหว่างทดสอบที่ยังไม่ได้ใส่ URL จริง
                    if (scriptURL === 'YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL') {
                        form.reset();
                        window.showModal('success-modal');
                        console.log('Simulating success since URL is placeholder.');
                    } else {
                        alert('เกิดข้อผิดพลาดในการบันทึกข้อมูล กรุณาลองใหม่อีกครั้ง');
                    }
                })
                .finally(() => {
                    // คืนค่าปุ่มกลับเป็นเหมือนเดิม
                    submitBtn.innerText = originalBtnText;
                    submitBtn.disabled = false;
                    submitBtn.style.opacity = '1';
                });
        };

        // ฟังก์ชันสำหรับเปิด-ปิด Modal
        window.showModal = function(modalId) {
            const modal = document.getElementById(modalId);
            modal.style.display = 'flex';
            // บังคับให้เบราว์เซอร์รับรู้การแสดงผลก่อนเพิ่ม class แอนิเมชัน
            void modal.offsetWidth;
            modal.classList.add('show');
        };

        window.closeModal = function(modalId) {
            const modal = document.getElementById(modalId);
            modal.classList.remove('show');
            setTimeout(() => {
                modal.style.display = 'none';
            }, 300);
        };

        // ฟังก์ชันเรียกหน้าต่างติดต่อเรา
        window.showContactModal = function() {
            window.showModal('contact-modal');
        };
        
        // ให้สีปุ่มหน้าแรกทำงานตั้งแต่โหลดเว็บเสร็จ
        document.addEventListener('DOMContentLoaded', () => {
            const homeNav = document.getElementById('nav-home');
            if (homeNav) {
                homeNav.classList.remove('text-nature-light');
                homeNav.classList.add('text-nature-green');
            }
        });
    </script>
</body>
</html>
