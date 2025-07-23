<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vighnaharta Eco-Friendly Ganesha</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary-green: #2e7d32;
            --secondary-green: #81c784;
            --accent-gold: #ffd700;
            --dark-brown: #5d4037;
            --light-beige: #f5f5dc;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f9f9f9;
            color: #333;
        }
        
        .navbar {
            background-color: var(--primary-green);
        }
        
        .navbar-brand {
            font-weight: 700;
            color: white !important;
        }
        
        .nav-link {
            color: rgba(255, 255, 255, 0.85) !important;
        }
        
        .nav-link:hover {
            color: var(--accent-gold) !important;
        }
        
        .hero-section {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://via.placeholder.com/1920x600') center/cover no-repeat;
            color: white;
            padding: 120px 0;
            text-align: center;
        }
        
        .language-selector {
            background-color: var(--dark-brown);
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 4px;
        }
        
        .product-card {
            border: none;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            background-color: white;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
        }
        
        .product-img {
            height: 200px;
            object-fit: cover;
        }
        
        .price-tag {
            background-color: var(--primary-green);
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-weight: bold;
        }
        
        .btn-booking {
            background-color: var(--primary-green);
            color: white;
            border: none;
            padding: 8px 20px;
            border-radius: 20px;
            transition: all 0.3s;
        }
        
        .btn-booking:hover {
            background-color: var(--dark-brown);
            transform: scale(1.05);
        }
        
        .feature-box {
            text-align: center;
            padding: 30px 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            transition: all 0.3s;
        }
        
        .feature-box:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            color: var(--primary-green);
            margin-bottom: 15px;
        }
        
        footer {
            background-color: var(--dark-brown);
            color: white;
            padding: 40px 0;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: var(--accent-gold);
        }
        
        .social-icons a {
            color: white;
            font-size: 1.5rem;
            margin-right: 15px;
            transition: color 0.3s;
        }
        
        .social-icons a:hover {
            color: var(--accent-gold);
        }
        
        .delivery-info {
            background-color: var(--light-beige);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 30px;
        }
        
        .marathi-text {
            font-family: 'Noto Sans Devanagari', sans-serif;
        }
    </style>
</head>
<body>
    <!-- Language Selection Bar -->
    <div class="bg-dark py-2 text-end">
        <select class="language-selector" id="languageSelector">
            <option value="en">English</option>
            <option value="mr">मराठी</option>
            <option value="hi">हिन्दी</option>
            <option value="ta">தமிழ்</option>
            <option value="te">తెలుగు</option>
            <option value="kn">ಕನ್ನಡ</option>
        </select>
    </div>

    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">
                <i class="fas fa-leaf me-2"></i>
                <span class="en">Vighnaharta Eco-Friendly Ganesha</span>
                <span class="mr marathi-text" style="display:none">विघ्नहर्ता इको-फ्रेंडली गणेशा</span>
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link en" href="#">Home</a>
                        <a class="nav-link mr" href="#" style="display:none">मुख्यपृष्ठ</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link en" href="#products">Products</a>
                        <a class="nav-link mr" href="#products" style="display:none">उत्पादने</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link en" href="#booking">Booking</a>
                        <a class="nav-link mr" href="#booking" style="display:none">बुकिंग</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link en" href="#about">About Us</a>
                        <a class="nav-link mr" href="#about" style="display:none">आमच्याबद्दल</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link en" href="#contact">Contact</a>
                        <a class="nav-link mr" href="#contact" style="display:none">संपर्क</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-section">
        <div class="container">
            <h1 class="en display-4 fw-bold mb-4">Eco-Friendly Ganesha Idols</h1>
            <h1 class="mr marathi-text display-4 fw-bold mb-4" style="display:none">इको-फ्रेंडली गणेश मूर्ती</h1>
            <p class="en lead mb-5">Celebrate Ganesh Chaturthi with our 100% biodegradable idols made from natural materials</p>
            <p class="mr marathi-text lead mb-5" style="display:none">नैसर्गिक साहित्यापासून बनवलेल्या 100% जैवविघटनशील मूर्तीसह गणेश चतुर्थी साजरी करा</p>
            <a href="#booking" class="btn btn-booking btn-lg en">Book Now</a>
            <a href="#booking" class="btn btn-booking btn-lg mr" style="display:none">आता बुक करा</a>
        </div>
    </section>

    <!-- Features Section -->
    <section class="py-5">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-seedling"></i>
                        </div>
                        <h3 class="en">Eco-Friendly Materials</h3>
                        <h3 class="mr" style="display:none">इको-फ्रेंडली साहित्य</h3>
                        <p class="en">Made from natural clay and POP that dissolves easily in water</p>
                        <p class="mr" style="display:none">नैसर्गिक माती आणि POP पासून बनवलेले जे पाण्यात सहज विरघळते</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-truck"></i>
                        </div>
                        <h3 class="en">Home Delivery</h3>
                        <h3 class="mr" style="display:none">घरपोच</h3>
                        <p class="en">Convenient delivery before Ganesh Chaturthi</p>
                        <p class="mr" style="display:none">गणेश चतुर्थीच्या आधी सोयीस्कर घरपोच</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-hand-holding-water"></i>
                        </div>
                        <h3 class="en">Water Soluble</h3>
                        <h3 class="mr" style="display:none">जलविद्राव्य</h3>
                        <p class="en">Dissolves completely without harming water bodies</p>
                        <p class="mr" style="display:none">जलाशयांना नुकसान न करता पूर्णपणे विरघळते</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section id="products" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-5 en">Our Products</h2>
            <h2 class="text-center mb-5 mr" style="display:none">आमची उत्पादने</h2>
            
            <div class="row">
                <!-- C-Series Products -->
                <div class="col-md-6">
                    <div class="card product-card">
                        <img src="https://via.placeholder.com/300x200?text=C-127+(10in)" class="card-img-top product-img" alt="Ganesha Idol">
                        <div class="card-body">
                            <h5 class="card-title">C-127 (10")</h5>
                            <p class="card-text en">Plaster of Paris idol with eco-friendly colors</p>
                            <p class="card-text mr" style="display:none">इको-फ्रेंडली रंगांसह POP मूर्ती</p>
                            <div class="d-flex justify-content-between align-items-center">
                                <span class="price-tag">₹1700</span>
                                <button class="btn btn-booking en">Book Now</button>
                                <button class="btn btn-booking mr" style="display:none">बुक करा</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="col-md-6">
                    <div class="card product-card">
                        <img src="https://via.placeholder.com/300x200?text=C-132+(12in)" class="card-img-top product-img" alt="Ganesha Idol">
                        <div class="card-body">
                            <h5 class="card-title">C-132 (12")</h5>
                            <p class="card-text en">Plaster of Paris idol with eco-friendly colors</p>
                            <p class="card-text mr" style="display:none">इको-फ्रेंडली रंगांसह POP मूर्ती</p>
                            <div class="d-flex justify-content-between align-items-center">
                                <span class="price-tag">₹2200</span>
                                <button class="btn btn-booking en">Book Now</button>
                                <button class="btn btn-booking mr" style="display:none">बुक करा</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Add more products similarly -->
            </div>
            
            <div class="text-center mt-4">
                <a href="#products" class="btn btn-outline-primary en">View All Products</a>
                <a href="#products" class="btn btn-outline-primary mr" style="display:none">सर्व उत्पादने पहा</a>
            </div>
        </div>
    </section>

    <!-- Booking Process Section -->
    <section id="booking" class="py-5">
        <div class="container">
            <h2 class="text-center mb-5 en">Easy Booking Process</h2>
            <h2 class="text-center mb-5 mr" style="display:none">सोपी बुकिंग प्रक्रिया</h2>
            
            <div class="row">
                <div class="col-md-6">
                    <div class="delivery-info">
                        <h4 class="en"><i class="fas fa-info-circle me-2"></i>Booking Information</h4>
                        <h4 class="mr" style="display:none"><i class="fas fa-info-circle me-2"></i>बुकिंग माहिती</h4>
                        <ul class="en">
                            <li>50% advance payment required at time of booking</li>
                            <li>Balance 50% to be paid at delivery</li>
                            <li>Delivery charges: ₹200 (Pune), ₹400 (PCMC)</li>
                            <li>Delivery starts one week before Ganesh Chaturthi</li>
                        </ul>
                        <ul class="mr" style="display:none">
                            <li>बुकिंगच्या वेळी ५०% अ‍ॅडव्हान्स पेमेंट आवश्यक</li>
                            <li>डिलिव्हरीच्या वेळी उर्वरित ५०% रक्कम द्यावी</li>
                            <li>डिलिव्हरी शुल्क: ₹२०० (पुणे), ₹४०० (PCMC)</li>
                            <li>गणेश चतुर्थीच्या एक आठवडा आधी डिलिव्हरी सुरू</li>
                        </ul>
                    </div>
                </div>
                
                <div class="col-md-6">
                    <div class="card">
                        <div class="card-header bg-primary text-white">
                            <h4 class="mb-0 en">Book Your Ganesha Idol</h4>
                            <h4 class="mb-0 mr" style="display:none">आपली गणेश मूर्ती बुक करा</h4>
                        </div>
                        <div class="card-body">
                            <form id="bookingForm">
                                <div class="mb-3">
                                    <label for="name" class="form-label en">Full Name</label>
                                    <label for="name" class="form-label mr" style="display:none">पूर्ण नाव</label>
                                    <input type="text" class="form-control" id="name" required>
                                </div>
                                <div class="mb-3">
                                    <label for="phone" class="form-label en">Phone Number</label>
                                    <label for="phone" class="form-label mr" style="display:none">फोन नंबर</label>
                                    <input type="tel" class="form-control" id="phone" required>
                                </div>
                                <div class="mb-3">
                                    <label for="email" class="form-label en">Email</label>
                                    <label for="email" class="form-label mr" style="display:none">ईमेल</label>
                                    <input type="email" class="form-control" id="email">
                                </div>
                                <div class="mb-3">
                                    <label for="address" class="form-label en">Delivery Address</label>
                                    <label for="address" class="form-label mr" style="display:none">डिलिव्हरी पत्ता</label>
                                    <textarea class="form-control" id="address" rows="3" required></textarea>
                                </div>
                                <div class="mb-3">
                                    <label for="product" class="form-label en">Select Idol</label>
                                    <label for="product" class="form-label mr" style="display:none">मूर्ती निवडा</label>
                                    <select class="form-select" id="product" required>
                                        <option value="" selected disabled en>Choose an idol</option>
                                        <option value="" selected disabled mr" style="display:none">मूर्ती निवडा</option>
                                        <option value="C-127">C-127 (10") - ₹1700</option>
                                        <option value="C-132">C-132 (12") - ₹2200</option>
                                        <option value="C-133">C-133 (12") - ₹2200</option>
                                        <!-- Add more options -->
                                    </select>
                                </div>
                                <div class="mb-3 form-check">
                                    <input type="checkbox" class="form-check-input" id="terms" required>
                                    <label class="form-check-label en" for="terms">I agree to the terms and conditions</label>
                                    <label class="form-check-label mr" style="display:none" for="terms">मी अटी व नियमांशी सहमत आहे</label>
                                </div>
                                <button type="submit" class="btn btn-booking w-100 en">Proceed to Payment</button>
                                <button type="submit" class="btn btn-booking w-100 mr" style="display:none">पेमेंट करा</button>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about" class="py-5 bg-light">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-md-6">
                    <h2 class="en">About Vighnaharta Eco-Friendly Ganesha</h2>
                    <h2 class="mr" style="display:none">विघ्नहर्ता इको-फ्रेंडली गणेशा बद्दल</h2>
                    <p class="en">We are committed to providing high-quality, eco-friendly Ganesha idols that dissolve completely in water without harming the environment. Our idols are made from natural materials like clay and Plaster of Paris with eco-friendly colors.</p>
                    <p class="mr" style="display:none">आम्ही पर्यावरणाला नुकसान न पोहोचवता पाण्यात पूर्णपणे विरघळणाऱ्या उच्च दर्जाच्या इको-फ्रेंडली गणेश मूर्ती पुरवण्यासाठी वचनबद्ध आहोत. आमच्या मूर्ती नैसर्गिक साहित्यापासून बनवल्या जातात जसे की माती आणि इको-फ्रेंडली रंगांसह POP.</p>
                </div>
                <div class="col-md-6">
                    <img src="https://via.placeholder.com/600x400?text=Workshop" class="img-fluid rounded" alt="Our Workshop">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-5">
        <div class="container">
            <h2 class="text-center mb-5 en">Contact Us</h2>
            <h2 class="text-center mb-5 mr" style="display:none">आमच्याशी संपर्क साधा</h2>
            
            <div class="row">
                <div class="col-md-6">
                    <div class="card mb-4">
                        <div class="card-body">
                            <h4 class="en"><i class="fas fa-map-marker-alt me-2"></i>Our Address</h4>
                            <h4 class="mr" style="display:none"><i class="fas fa-map-marker-alt me-2"></i>आमचा पत्ता</h4>
                            <p>S. No. 2/7/2, Shop No. 1,<br>
                            Lodha Complex CHS, On Shanti Dham Road,<br>
                            Dhankawadi, Pune – 411043</p>
                        </div>
                    </div>
                    
                    <div class="card">
                        
