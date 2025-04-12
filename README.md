
<!DOCTYPE html>
<html lang="bn">
<head>
<script type='text/javascript' src='//pitsensation.com/03/e3/09/03e309a5d1273a0ef13e556014af27f6.js'></script>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>প্রিমিয়াম অ্যাডাল্ট কমিউনিটি</title>
    <style>
        :root {
            --primary-color: #ff4757;
            --secondary-color: #ff6b81;
            --dark-color: #2f3542;
            --light-color: #f1f2f6;
            --warning-color: #ff7f50;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f8f9fa;
            margin: 0;
            padding: 0;
            color: #333;
            line-height: 1.6;
        }
        
        .header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 2rem 1rem;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }
        
        .header h1 {
            margin: 0;
            font-size: 2.5rem;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
        }
        
        .header p {
            margin: 0.5rem 0 0;
            font-size: 1.1rem;
            opacity: 0.9;
        }
        
        .profile-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            padding: 2rem;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .profile-card {
            background: white;
            border-radius: 12px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.08);
            overflow: hidden;
            transition: all 0.3s ease;
            position: relative;
        }
        
        .profile-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 20px rgba(0,0,0,0.15);
        }
        
        .profile-img-container {
            position: relative;
            height: 300px;
            overflow: hidden;
        }
        
        .profile-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .profile-card:hover .profile-img {
            transform: scale(1.05);
        }
        
        .profile-info {
            padding: 1.5rem;
            text-align: center;
        }
        
        .profile-info h3 {
            margin: 0 0 0.5rem;
            color: var(--dark-color);
            font-size: 1.4rem;
        }
        
        .profile-info p {
            margin: 0 0 1rem;
            color: #666;
            font-size: 0.95rem;
        }
        
        .join-btn {
            background: linear-gradient(135deg, #ff6b6b, #ff4757);
            color: white;
            border: none;
            padding: 14px 30px;
            border-radius: 8px;
            cursor: pointer;
            font-weight: bold;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            width: 100%;
            letter-spacing: 0.5px;
            text-transform: uppercase;
            text-decoration: none;
            display: block;
            position: relative;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
            margin-top: 15px;
        }
        
        .join-btn:hover {
            background: linear-gradient(135deg, #ff4757, #ff6b6b);
            box-shadow: 0 6px 20px rgba(255, 71, 87, 0.6);
            transform: translateY(-2px);
        }
        
        .join-btn:active {
            transform: translateY(0);
        }
        
        .join-btn::after {
            content: "";
            position: absolute;
            top: -50%;
            left: -60%;
            width: 200%;
            height: 200%;
            background: rgba(255,255,255,0.2);
            transform: rotate(30deg);
            transition: all 0.3s;
        }
        
        .join-btn:hover::after {
            left: 100%;
        }
        
        .district-notice {
            background: linear-gradient(135deg, #4b6cb7, #182848);
            color: white;
            padding: 1rem;
            border-radius: 8px;
            text-align: center;
            margin: 1rem auto;
            max-width: 1200px;
            font-size: 1.2rem;
            font-weight: bold;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            border-left: 5px solid #ff4757;
        }
        
        .age-gate {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.95);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 1000;
            color: white;
            backdrop-filter: blur(5px);
        }
        
        .age-box {
            background: var(--dark-color);
            padding: 3rem;
            border-radius: 15px;
            text-align: center;
            max-width: 500px;
            width: 90%;
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .age-box h2 {
            margin-top: 0;
            color: white;
            font-size: 1.8rem;
        }
        
        .age-box p {
            margin-bottom: 2rem;
            font-size: 1.1rem;
            opacity: 0.9;
        }
        
        .age-btn {
            padding: 12px 30px;
            margin: 0 10px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: bold;
            font-size: 1rem;
            transition: all 0.3s ease;
            border: none;
        }
        
        .age-btn.confirm {
            background: var(--primary-color);
            color: white;
        }
        
        .age-btn.deny {
            background: #666;
            color: white;
        }
        
        .age-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0,0,0,0.2);
        }
        
        .hidden {
            display: none;
        }
        
        .warning {
            background-color: #fff8f6;
            color: var(--warning-color);
            font-weight: bold;
            margin: 0 auto;
            padding: 1rem;
            border-radius: 8px;
            text-align: center;
            max-width: 1200px;
            border-left: 5px solid var(--warning-color);
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            animation: pulse 2s infinite;
        }
        
        .data-notice {
            background-color: #e3f2fd;
            color: #1976d2;
            padding: 0.8rem;
            border-radius: 6px;
            margin: 0.5rem auto;
            font-size: 0.9rem;
            text-align: center;
            border-left: 4px solid #1976d2;
            max-width: 1200px;
        }
        
        .login-notice {
            color: #ff4757;
            font-size: 0.85rem;
            margin-top: 0.5rem;
            font-style: italic;
        }
        
        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.8; }
            100% { opacity: 1; }
        }
        
        .warning-icon {
            font-size: 1.5rem;
        }
        
        footer {
            background: var(--dark-color);
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 2rem;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 1rem;
        }
        
        .footer-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-links a:hover {
            color: var(--primary-color);
        }
        
        @media (max-width: 768px) {
            .profile-container {
                grid-template-columns: 1fr;
                padding: 1rem;
            }
            
            .header h1 {
                font-size: 2rem;
            }
            
            .age-box {
                padding: 2rem 1rem;
            }
            
            .age-btn {
                display: block;
                width: 100%;
                margin: 10px 0;
            }
            
            .district-notice {
                font-size: 1rem;
                padding: 0.8rem;
            }
        }
    </style>
</head>
<body>
    <!-- বয়স ভেরিফিকেশন পপআপ -->
    <div class="age-gate" id="ageGate">
        <div class="age-box">
            <h2>বয়স সীমাবদ্ধতা</h2>
            <p>এই কমিউনিটি শুধুমাত্র ১৮+ বয়সের সদস্যদের জন্য</p>
            <p>আপনার বয়স ১৮ বা তার বেশি?</p>
            <button class="age-btn confirm" onclick="verifyAge(true)">হ্যাঁ, আমি প্রাপ্তবয়স্ক</button>
            <button class="age-btn deny" onclick="verifyAge(false)">না, আমি প্রাপ্তবয়স্ক নই</button>
        </div>
    </div>

    <!-- মূল কন্টেন্ট -->
    <div class="header">
        <h1>প্রিমিয়াম অ্যাডাল্ট কমিউনিটি</h1>
        <p>শুধুমাত্র ভেরিফাইড প্রাপ্তবয়স্ক সদস্যদের জন্য</p>
    </div>

    <div class="warning">
        <span class="warning-icon">⚠️</span>
        <span>এই সাইটের কন্টেন্ট শুধুমাত্র প্রাপ্তবয়স্কদের জন্য। ১৮ বছরের কম বয়সীদের প্রবেশ নিষিদ্ধ।</span>
    </div>

    <div class="data-notice">
        ⚠️ WiFi নেটওয়ার্কে জয়েন করা সম্ভব নয়। মোবাইল ডাটা ব্যবহার করুন।
    </div>

    <div class="district-notice">
        এখানে ৬৪ জেলার মেয়েরা আছে ভিডিও কলে কথা বলার জন্য
    </div>

    <div class="profile-container">
        <!-- প্রোফাইল কার্ড ১ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhN0M8SQ98ROxFceQlr7_QbYENk4hSUdmtxOIAAJRBgGSEpS7vxqK_d351y_eHW6XTc5DTpX5Fj8Q6qKYQYgGRqIDKDEQZ_edRs9B1TqiNBR9qJt58raQbB9fxk0ExNuz4kk2BqLvnrjjWOH5sXg__AaLuM6-GhViaYtEVVRW6WtJOQbPpHRIWySKFr5vgJ/s251/1000013440.jpg" alt="প্রোফাইল ১" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>তানিয়া</h3>
                <p>২৫ বছর, ঢাকা</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://pitsensation.com/br0cfv9q?key=870386e6feca6d0162aa15d309fea1b5" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>

        <!-- প্রোফাইল কার্ড ২ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjq42eBbH289g-G_Z7pGkSWROU9Nr3ptxsWJcrTrUvpCt5z2NSSpBKTqpfJu3tixMNgRRtuiMg4yWSfJIcHFe83f-sjmPf3s3V4q3fuiIg8CzdtOkAfThL0hqTMVHxvTdOaay4DKMzo19SlnXuQ5kKSI-l9q-5dw6d3I5SQMxDg0kKemNXMg47hc1BAedyr/s225/1000013437.jpg" alt="প্রোফাইল ২" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>প্রিয়া</h3>
                <p>২২ বছর, চট্টগ্রাম</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://whoockeg.top/4/8868785" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>

        <!-- প্রোফাইল কার্ড ৩ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhjhUjuTjWZ5NpbczsPGRn11pLsITkmYVgaUTmPJ833jNAJU3TNBhyxXgWbkxVovFmkq-MtXrf0nZnmviiD_YOV3xoPZ5lmBG0Iv41u3CrxZ_aJdvDcfCA0VcD-Fa9L9HOD5OGBfsVMHAJGrc59BIbg7WUfAeW2u6L_1u3529CguZ2WU3zKS7bKxvKWCiaI/s225/1000013436.jpg" alt="প্রোফাইল ৩" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>মিতু</h3>
                <p>২৭ বছর, সিলেট</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://pitsensation.com/br0cfv9q?key=870386e6feca6d0162aa15d309fea1b5" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>

        <!-- প্রোফাইল কার্ড ৪ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjafUEahdRZJAwzOvUIm2tIqPv55DqpehlMQBKg-Y_umMRrO6EcBy-ao2ZQ3uAqmfx0MGiAYEsJP5kgkwnb0uCUY5ieF1HY0LLEUMmmh9WYS7oBe8uYZUH2v7wPEuKJe41nJr5ipjy9nYmugDa4Qh5FBIQElpGhWRFuDkYFGSQtlWJ3EQF6hhnUb5tPbAKI/s299/1000013433.jpg" alt="প্রোফাইল ৪" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>নাবিলা</h3>
                <p>২৩ বছর, রাজশাহী</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://whoockeg.top/4/8868785" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>
        
        <!-- প্রোফাইল কার্ড ৫ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjELtmii4qaYRucGa-8cl748dTph4DLLCl1jeegJ72EMb5SxvXCuqlGDLgzI6Z8txFz9CABwhL7iTRZPW4lgFOPPD5PQO7WnLtnKqbsK_a3O_tPpouLsr56y8GM-nktQoTak9NaRtI7Ww63DHnIqa_QyghE84bpXpsl0EMfSlklYUjSYyxHxfNopCVTdiyP/s299/1000013430.jpg" alt="প্রোফাইল ৫" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>জারা</h3>
                <p>২৪ বছর, খুলনা</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://pitsensation.com/br0cfv9q?key=870386e6feca6d0162aa15d309fea1b5" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>
        
        <!-- প্রোফাইল কার্ড ৬ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiFkjZKZPtiAfWPilEAX18hJEmOA_Fw_vHDXl15i9l8bDz4Pz69rjJKgnlGZUPXMK8b7QABgyE9ZP3aI-NVDQi4kMsBIpkmPUmdmVw_FH0OV4xWkvGsPxSF4gzv160fmiBXX_k019-iDTfGflPb6MHo_MROMuv1rezyBnP5OPx3rGI3UG76QH7bjPl30Pwl/s275/1000013432.jpg" alt="প্রোফাইল ৬" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>তিশা</h3>
                <p>২১ বছর, বরিশাল</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://whoockeg.top/4/8868785" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>
        
        <!-- প্রোফাইল কার্ড ৭ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh-V7IpxTjDAsY_RUSGXMZaUJ8GH1uOWSXoGhln2z9icuT1i3IOpusp7vkVO-XzxVMXCIEV_HPWmtLiMI14ShqYr19SlNJaKIi_u6WnJoeZX7sR1a4reTmQGtRiGe57FqSm5eZCXTLQ6hE67hXYtWS_KhnNJSosbv6lZ0P-og80KDY0gG3x_5iPKEA3FQ7G/s299/1000013435.jpg" alt="প্রোফাইল ৭" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>মিম</h3>
                <p>২৬ বছর, রংপুর</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://pitsensation.com/br0cfv9q?key=870386e6feca6d0162aa15d309fea1b5" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>
        
        <!-- প্রোফাইল কার্ড ৮ -->
        <div class="profile-card">
            <div class="profile-img-container">
                <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEih_v6Qpjs2_A-YuG_CRPNTV4jG9Oc0QdKkf-5vBKXwjz5xVxl3qV2QD3SO9NXV8ODbOkfeevgNvhP5Vc7fs3FoIeeseGlhzY30d6KlhE_IWu4CFvkNU9MsnzbNmsQZwFWNYxshVUH1XFdMEtqSGRyh5W0S0MtHhCzvM3vnXrOI5cGM79-L69tiHdAaksIG/s299/1000013431.jpg" alt="প্রোফাইল ৮" class="profile-img">
            </div>
            <div class="profile-info">
                <h3>নাজিয়া</h3>
                <p>২৫ বছর, কুমিল্লা</p>
                <div class="login-notice">কোনো সাইড এ নিয়ে গেলে লগিং করে আবার চেষ্টা করুন</div>
                <a href="https://whoockeg.top/4/8868785" class="join-btn">জয়েন প্রিমিয়াম গ্রুপ</a>
            </div>
        </div>
    </div>

    <footer>
        <div class="footer-links">
            <a href="#">প্রাইভেসি পলিসি</a>
            <a href="#">টার্মস অফ সার্ভিস</a>
            <a href="#">যোগাযোগ</a>
        </div>
        <p>&copy; ২০২৪ প্রিমিয়াম কমিউনিটি. সকল স্বত্ব সংরক্ষিত</p>
    </footer>

    <script>
        // বয়স ভেরিফিকেশন
        function verifyAge(isAdult) {
            const ageGate = document.getElementById('ageGate');
            
            if(isAdult) {
                // এনিমেশন সহ লুকানো
                ageGate.style.animation = "fadeIn 0.5s ease reverse";
                setTimeout(() => {
                    ageGate.classList.add('hidden');
                }, 400);
                
                localStorage.setItem('ageVerified', 'true');
            } else {
                window.location.href = 'https://www.google.com';
            }
        }

        // প্রথম লোডে চেক
        window.onload = function() {
            if(localStorage.getItem('ageVerified') === 'true') {
                document.getElementById('ageGate').classList.add('hidden');
            }
        };
    </script>
</body>
                                                                                        </html>
