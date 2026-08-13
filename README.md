<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>แนะนำตัว - ชื่อของคุณ</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Sarabun', 'Kanit', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .card {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            max-width: 500px;
            width: 100%;
            overflow: hidden;
            animation: slideUp 0.8s ease;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 40px 30px;
            text-align: center;
            position: relative;
        }

        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 5px solid white;
            object-fit: cover;
            margin-bottom: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
        }

        .name {
            color: white;
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .title {
            color: rgba(255,255,255,0.9);
            font-size: 16px;
        }

        .content {
            padding: 30px;
        }

        .section {
            margin-bottom: 25px;
        }

        .section-title {
            color: #667eea;
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .section-title::before {
            content: '';
            display: inline-block;
            width: 4px;
            height: 20px;
            background: #667eea;
            border-radius: 2px;
        }

        .bio {
            color: #555;
            line-height: 1.8;
            font-size: 15px;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-tag {
            background: #f0f0f0;
            color: #667eea;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 13px;
            font-weight: 500;
            transition: all 0.3s;
        }

        .skill-tag:hover {
            background: #667eea;
            color: white;
            transform: translateY(-2px);
        }

        .contact {
            display: flex;
            gap: 12px;
            justify-content: center;
            margin-top: 10px;
        }

        .contact-btn {
            padding: 10px 24px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 14px;
            font-weight: 600;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
        }

        .btn-primary {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
        }

        .btn-secondary {
            background: #f0f0f0;
            color: #555;
        }

        .btn-secondary:hover {
            background: #e0e0e0;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid #eee;
        }

        .social-links a {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: #f0f0f0;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            color: #667eea;
            font-size: 18px;
            transition: all 0.3s;
        }

        .social-links a:hover {
            background: #667eea;
            color: white;
            transform: translateY(-3px);
        }

        .stats {
            display: flex;
            justify-content: space-around;
            padding: 20px 0;
            border-top: 1px solid #eee;
            border-bottom: 1px solid #eee;
            margin-bottom: 20px;
        }

        .stat-item {
            text-align: center;
        }

        .stat-number {
            font-size: 24px;
            font-weight: bold;
            color: #667eea;
        }

        .stat-label {
            font-size: 12px;
            color: #888;
            margin-top: 2px;
        }

        /* เอฟเฟกต์พิมพ์ข้อความ */
        .typewriter {
            overflow: hidden;
            border-right: 2px solid #667eea;
            white-space: nowrap;
            animation: typing 3s steps(30) 1s forwards, blink 0.75s step-end infinite;
            width: 0;
        }

        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes blink {
            50% { border-color: transparent }
        }

        @media (max-width: 480px) {
            .card {
                margin: 10px;
            }
            .name {
                font-size: 24px;
            }
        }
    </style>
    <!-- โหลดฟอนต์ไทย -->
    <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="card">
        <!-- ส่วนหัว -->
        <div class="header">
            <!-- เปลี่ยนเป็นรูปของคุณ -->
            <img [src="https://via.placeholder.com/120" alt]="รูปโปรไฟล์" class="avatar">
            <div class="name">กลทีบ์ ศรีบุญเรือ</div>
            <div class="title"นักศึกษา</div>
        </div>

        <!-- ส่วนเนื้อหา -->
        <div class="content">
            <!-- สถิติ -->
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">5+</div>
                    <div class="stat-label">ปีประสบการณ์</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">50+</div>
                    <div class="stat-label">โปรเจกต์</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">100+</div>
                    <div class="stat-label">ลูกค้า</div>
                </div>
            </div>

            <!-- เกี่ยวกับตัวฉัน -->
            <div class="section">
                <div class="section-title">เกี่ยวกับฉัน</div>
                <p class="bio">
                    สวัสดีครับ/ค่ะ ฉันคือ [ชื่อของคุณ] มีความสนใจและความเชี่ยวชาญในด้าน [ระบุสาขา] 
                    ฉันมุ่งมั่นที่จะสร้างสรรค์ผลงานที่มีคุณภาพและตอบโจทย์ความต้องการของผู้ใช้งาน
                </p>
            </div>

            <!-- ทักษะ -->
            <div class="section">
                <div class="section-title">ทักษะ</div>
                <div class="skills">
                    <span class="skill-tag">HTML/CSS</span>
                    <span class="skill-tag">JavaScript</span>
                    <span class="skill-tag">React</span>
                    <span class="skill-tag">UI/UX Design</span>
                    <span class="skill-tag">Python</span>
                    <span class="skill-tag">การวิเคราะห์ข้อมูล</span>
                </div>
            </div>

            <!-- ปุ่มติดต่อ -->
            <div class="contact">
                <a href="mailto:your@email.com" class="contact-btn btn-primary">📧 ส่งอีเมล</a>
                <a href="tel:0812345678" class="contact-btn btn-secondary">📞 โทรศัพท์</a>
            </div>

            <!-- โซเชียลมีเดีย -->
            <div class="social-links">
                <a href="#" title="Facebook">f</a>
                <a href="#" title="Twitter">𝕏</a>
                <a href="#" title="LinkedIn">in</a>
                <a href="#" title="GitHub">gh</a>
                <a href="#" title="Instagram">📷</a>
            </div>
        </div>
    </div>

    <script>
        // เอฟเฟกต์เลื่อนเข้าเมื่อโหลดหน้า
        document.addEventListener('DOMContentLoaded', function() {
            const card = document.querySelector('.card');
            
            // เพิ่มเอฟเฟกต์ hover ให้กับการ์ด
            card.addEventListener('mousemove', function(e) {
                const rect = card.getBoundingClientRect();
                const x = e.clientX - rect.left;
                const y = e.clientY - rect.top;
                
                card.style.setProperty('--mouse-x', x + 'px');
                card.style.setProperty('--mouse-y', y + 'px');
            });
        });

        // ฟังก์ชันคัดลอกอีเมล
        function copyEmail() {
            navigator.clipboard.writeText('your@email.com');
            alert('คัดลอกอีเมลแล้ว!');
        }
    </script>
</body>
</html>
