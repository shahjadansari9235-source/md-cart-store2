 md-cart-store2
https://shahjadansari9235-source.github.io
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MD Cart - India's Largest Online Shopping Store</title>
    <meta name="description" content="MD Cart - India's No. 1 Online Shopping Destination. Shop for Electronics, Fashion, Home, Grocery, Mobiles & More. Best Prices & Free Shipping.">
    <meta name="keywords" content="online shopping, ecommerce, MD Cart, flipkart alternative, amazon india, shop online">
    <meta name="author" content="MD Cart">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #2874f0;
            --primary-dark: #1c60d1;
            --secondary: #fb641b;
            --accent: #ff9f00;
            --success: #388e3c;
            --light: #f5f5f5;
            --dark: #212121;
            --gray: #878787;
            --border: #e0e0e0;
            --shadow: 0 1px 2px 0 rgba(0,0,0,.2);
            --shadow-lg: 0 4px 12px 0 rgba(0,0,0,.12);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            background-color: #f1f3f6;
            color: var(--dark);
            line-height: 1.6;
        }

        /* Utility Classes */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .btn {
            padding: 12px 24px;
            border-radius: 2px;
            font-weight: 600;
            cursor: pointer;
            border: none;
            transition: all 0.3s;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            font-size: 14px;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
        }

        .btn-primary:hover {
            background: var(--primary-dark);
            box-shadow: var(--shadow);
        }

        .btn-secondary {
            background: var(--secondary);
            color: white;
        }

        .btn-secondary:hover {
            background: #e55a17;
        }

        .btn-outline {
            background: white;
            color: var(--primary);
            border: 1px solid var(--primary);
        }

        .btn-outline:hover {
            background: #f0f8ff;
        }

        /* Login Page */
        .login-page {
            min-height: 100vh;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .login-card {
            background: white;
            border-radius: 8px;
            box-shadow: var(--shadow-lg);
            width: 100%;
            max-width: 400px;
            padding: 40px;
            text-align: center;
        }

        .brand-logo {
            font-size: 42px;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .brand-name {
            font-size: 32px;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 5px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .brand-name .plus {
            color: var(--accent);
            background: #ffeaa7;
            padding: 2px 8px;
            border-radius: 4px;
            font-size: 14px;
        }

        .tagline {
            color: var(--gray);
            margin-bottom: 30px;
        }

        .login-form input {
            width: 100%;
            padding: 14px;
            margin-bottom: 16px;
            border: 1px solid var(--border);
            border-radius: 4px;
            font-size: 14px;
            transition: border 0.3s;
        }

        .login-form input:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 2px rgba(40, 116, 240, 0.1);
        }

        .login-btn {
            width: 100%;
            background: var(--primary);
            color: white;
            border: none;
            padding: 14px;
            border-radius: 4px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }

        .login-btn:hover {
            background: var(--primary-dark);
        }

        .or-divider {
            text-align: center;
            margin: 20px 0;
            color: var(--gray);
            position: relative;
        }

        .or-divider::before,
        .or-divider::after {
            content: '';
            position: absolute;
            top: 50%;
            width: 45%;
            height: 1px;
            background: var(--border);
        }

        .or-divider::before {
            left: 0;
        }

        .or-divider::after {
            right: 0;
        }

        .signup-btn {
            width: 100%;
            background: white;
            color: var(--primary);
            border: 1px solid var(--primary);
            padding: 14px;
            border-radius: 4px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
        }

        .signup-btn:hover {
            background: #f0f8ff;
        }

        .guest-btn {
            width: 100%;
            background: transparent;
            color: var(--primary);
            border: none;
            padding: 14px;
            font-size: 14px;
            cursor: pointer;
            margin-top: 15px;
        }

        .guest-btn:hover {
            text-decoration: underline;
        }

        /* Main Store */
        .main-store {
            display: none;
        }

        /* Top Bar */
        .top-bar {
            background: var(--primary);
            color: white;
            padding: 8px 0;
            font-size: 13px;
        }

        .top-bar-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .top-links {
            display: flex;
            gap: 20px;
        }

        .top-links a {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .top-links a:hover {
            text-decoration: underline;
        }

        /* Header */
        .main-header {
            background: white;
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header-content {
            display: flex;
            align-items: center;
            padding: 12px 0;
            gap: 20px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 8px;
            text-decoration: none;
        }

        .logo-icon {
            font-size: 28px;
            color: var(--primary);
        }

        .logo-text {
            font-size: 22px;
            font-weight: 800;
            color: var(--primary);
            font-style: italic;
        }

        .logo-text span {
            color: var(--accent);
        }

        .search-bar {
            flex: 1;
            position: relative;
        }

        .search-input {
            width: 100%;
            padding: 12px 50px 12px 16px;
            border: 1px solid var(--border);
            border-radius: 2px;
            font-size: 14px;
            background: #f0f5ff;
        }

        .search-input:focus {
            outline: none;
            background: white;
        }

        .search-btn {
            position: absolute;
            right: 0;
            top: 0;
            height: 100%;
            width: 50px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 0 2px 2px 0;
            cursor: pointer;
        }

        .header-actions {
            display: flex;
            gap: 25px;
            align-items: center;
        }

        .action-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            color: var(--dark);
            text-decoration: none;
            font-size: 12px;
            font-weight: 600;
        }

        .action-icon {
            font-size: 20px;
            margin-bottom: 4px;
            color: var(--dark);
        }

        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background: var(--secondary);
            color: white;
            font-size: 10px;
            padding: 2px 6px;
            border-radius: 50%;
            min-width: 18px;
            text-align: center;
        }

        .user-menu {
            position: relative;
        }

        .user-avatar {
            width: 36px;
            height: 36px;
            border-radius: 50%;
            background: var(--primary);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
            cursor: pointer;
        }

        /* Categories Bar */
        .categories-bar {
            background: white;
            border-bottom: 1px solid var(--border);
        }

        .categories {
            display: flex;
            overflow-x: auto;
            padding: 12px 0;
            gap: 25px;
        }

        .category-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-decoration: none;
            color: var(--dark);
            font-size: 13px;
            font-weight: 600;
            min-width: 70px;
        }

        .category-icon {
            width: 60px;
            height: 60px;
            background: #f5f5f5;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 8px;
            font-size: 24px;
            color: var(--primary);
            transition: transform 0.3s;
        }

        .category-item:hover .category-icon {
            transform: scale(1.1);
            background: #e8f0fe;
        }

        /* Hero Banner */
        .hero-section {
            padding: 20px 0;
        }

        .hero-slider {
            background: white;
            border-radius: 4px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .hero-slide {
            display: flex;
            align-items: center;
            padding: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .hero-content {
            flex: 1;
            padding: 40px;
        }

        .hero-title {
            font-size: 36px;
            font-weight: 800;
            margin-bottom: 15px;
        }

        .hero-subtitle {
            font-size: 18px;
            margin-bottom: 25px;
            opacity: 0.9;
        }

        .hero-image {
            flex: 1;
            text-align: center;
        }

        .hero-image img {
            max-width: 100%;
            height: auto;
        }

        /* Products Grid */
        .products-section {
            margin: 20px 0;
        }

        .section-header {
            background: white;
            padding: 15px 20px;
            margin-bottom: 10px;
            border-radius: 4px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: var(--shadow);
        }

        .section-title {
            font-size: 22px;
            font-weight: 700;
            color: var(--dark);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .view-all {
            color: var(--primary);
            text-decoration: none;
            font-weight: 600;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
            gap: 15px;
        }

        .product-card {
            background: white;
            border-radius: 4px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: transform 0.3s, box-shadow 0.3s;
            position: relative;
        }

        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .product-badge {
            position: absolute;
            top: 10px;
            left: 10px;
            background: var(--success);
            color: white;
            padding: 4px 8px;
            border-radius: 2px;
            font-size: 11px;
            font-weight: 600;
            z-index: 1;
        }

        .product-badge.sale {
            background: var(--secondary);
        }

        .product-badge.new {
            background: var(--accent);
        }

        .product-image {
            height: 200px;
            background: #f5f5f5;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            position: relative;
        }

        .product-image img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        .wishlist-btn {
            position: absolute;
            top: 10px;
            right: 10px;
            background: white;
            border: none;
            width: 36px;
            height: 36px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            box-shadow: var(--shadow);
            color: var(--gray);
            transition: all 0.3s;
        }

        .wishlist-btn:hover {
            color: #ff4757;
        }

        .wishlist-btn.active {
            color: #ff4757;
        }

        .product-details {
            padding: 15px;
        }

        .product-title {
            font-size: 14px;
            font-weight: 600;
            color: var(--dark);
            margin-bottom: 8px;
            display: -webkit-box;
            -webkit-line-clamp: 2;
            -webkit-box-orient: vertical;
            overflow: hidden;
        }

        .product-brand {
            color: var(--gray);
            font-size: 12px;
            margin-bottom: 8px;
        }

        .product-rating {
            display: flex;
            align-items: center;
            gap: 5px;
            margin-bottom: 10px;
        }

        .rating-stars {
            color: var(--accent);
            font-size: 12px;
        }

        .rating-count {
            color: var(--gray);
            font-size: 12px;
        }

        .price-section {
            display: flex;
            align-items: center;
            gap: 8px;
            margin-bottom: 12px;
        }

        .current-price {
            font-size: 18px;
            font-weight: 700;
            color: var(--dark);
        }

        .original-price {
            font-size: 14px;
            color: var(--gray);
            text-decoration: line-through;
        }

        .discount {
            color: var(--success);
            font-size: 12px;
            font-weight: 600;
        }

        .add-to-cart {
            width: 100%;
            background: var(--primary);
            color: white;
            border: none;
            padding: 10px;
            border-radius: 2px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }

        .add-to-cart:hover {
            background: var(--primary-dark);
        }

        .buy-now {
            width: 100%;
            background: var(--accent);
            color: white;
            border: none;
            padding: 10px;
            border-radius: 2px;
            font-weight: 600;
            cursor: pointer;
            margin-top: 8px;
            transition: background 0.3s;
        }

        .buy-now:hover {
            background: #e59400;
        }

        /* Footer */
        .main-footer {
            background: #172337;
            color: white;
            padding: 40px 0 20px;
            margin-top: 40px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-section h3 {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 20px;
            color: #878787;
            text-transform: uppercase;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: white;
            text-decoration: none;
            font-size: 13px;
            opacity: 0.8;
            transition: opacity 0.3s;
        }

        .footer-links a:hover {
            opacity: 1;
            text-decoration: underline;
        }

        .footer-bottom {
            border-top: 1px solid #2d3e50;
            padding-top: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 13px;
            opacity: 0.8;
        }

        .social-links {
            display: flex;
            gap: 15px;
        }

        .social-links a {
            color: white;
            font-size: 18px;
            opacity: 0.8;
            transition: opacity 0.3s;
        }

        .social-links a:hover {
            opacity: 1;
        }

        /* Cart Sidebar */
        .cart-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 2000;
            display: none;
        }

        .cart-overlay.active {
            display: block;
        }

        .cart-sidebar {
            position: fixed;
            top: 0;
            right: -400px;
            width: 100%;
            max-width: 400px;
            height: 100%;
            background: white;
            z-index: 2001;
            transition: right 0.3s ease;
            display: flex;
            flex-direction: column;
        }

        .cart-sidebar.active {
            right: 0;
        }

        .cart-header {
            padding: 20px;
            border-bottom: 1px solid var(--border);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .cart-title {
            font-size: 18px;
            font-weight: 700;
            color: var(--dark);
        }

        .close-cart {
            background: none;
            border: none;
            font-size: 20px;
            cursor: pointer;
            color: var(--gray);
        }

        .cart-items {
            flex: 1;
            overflow-y: auto;
            padding: 20px;
        }

        .cart-item {
            display: flex;
            gap: 15px;
            padding: 15px 0;
            border-bottom: 1px solid var(--border);
        }

        .cart-item:last-child {
            border-bottom: none;
        }

        .cart-item-image {
            width: 80px;
            height: 80px;
            background: #f5f5f5;
            border-radius: 4px;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
        }

        .cart-item-image img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        .cart-item-details {
            flex: 1;
        }

        .cart-item-title {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 5px;
        }

        .cart-item-price {
            font-size: 16px;
            font-weight: 700;
            color: var(--dark);
            margin-bottom: 10px;
        }

        .cart-item-actions {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .quantity-btn {
            width: 28px;
            height: 28px;
            border-radius: 50%;
            border: 1px solid var(--border);
            background: white;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .quantity-btn:hover {
            background: #f5f5f5;
        }

        .quantity {
            min-width: 30px;
            text-align: center;
        }

        .remove-item {
            background: none;
            border: none;
            color: var(--primary);
            cursor: pointer;
            font-size: 12px;
            margin-left: auto;
        }

        .remove-item:hover {
            text-decoration: underline;
        }

        .cart-footer {
            padding: 20px;
            border-top: 1px solid var(--border);
            background: white;
        }

        .cart-summary {
            margin-bottom: 20px;
        }

        .summary-row {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
            font-size: 14px;
        }

        .summary-row.total {
            font-size: 18px;
            font-weight: 700;
            border-top: 1px solid var(--border);
            padding-top: 15px;
            margin-top: 15px;
        }

        .checkout-btn {
            width: 100%;
            background: var(--accent);
            color: white;
            border: none;
            padding: 14px;
            border-radius: 2px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }

        .checkout-btn:hover {
            background: #e59400;
        }

        .empty-cart {
            text-align: center;
            padding: 40px 20px;
            color: var(--gray);
        }

        .empty-cart i {
            font-size: 60px;
            margin-bottom: 20px;
            opacity: 0.3;
        }

        /* Product Modal */
        .product-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 3000;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .product-modal.active {
            display: flex;
        }

        .modal-content {
            background: white;
            border-radius: 8px;
            max-width: 900px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
        }

        .modal-close {
            position: absolute;
            top: 20px;
            right: 20px;
            background: white;
            border: none;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 20px;
            color: var(--dark);
            z-index: 1;
            box-shadow: var(--shadow);
        }

        .modal-body {
            display: flex;
            padding: 30px;
            gap: 30px;
        }

        .modal-images {
            flex: 1;
        }

        .main-image {
            width: 100%;
            height: 400px;
            background: #f5f5f5;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }

        .main-image img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        .image-thumbnails {
            display: flex;
            gap: 10px;
            overflow-x: auto;
        }

        .thumbnail {
            width: 80px;
            height: 80px;
            background: #f5f5f5;
            border-radius: 4px;
            cursor: pointer;
            border: 2px solid transparent;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .thumbnail.active {
            border-color: var(--primary);
        }

        .thumbnail img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        .modal-details {
            flex: 1;
        }

        .modal-title {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 10px;
            color: var(--dark);
        }

        .modal-rating {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 20px;
        }

        .modal-price {
            font-size: 28px;
            font-weight: 700;
            color: var(--dark);
            margin-bottom: 20px;
        }

        .modal-offers {
            margin-bottom: 20px;
        }

        .offer-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 8px;
            color: var(--success);
            font-size: 14px;
        }

        .modal-specs {
            margin-bottom: 20px;
        }

        .spec-item {
            display: flex;
            margin-bottom: 8px;
            font-size: 14px;
        }

        .spec-label {
            width: 150px;
            color: var(--gray);
        }

        .spec-value {
            flex: 1;
            color: var(--dark);
        }

        .modal-actions {
            display: flex;
            gap: 10px;
            margin-top: 30px;
        }

        /* Notification */
        .notification {
            position: fixed;
            top: 100px;
            right: 20px;
            background: var(--success);
            color: white;
            padding: 12px 24px;
            border-radius: 4px;
            box-shadow: var(--shadow-lg);
            display: none;
            align-items: center;
            gap: 10px;
            z-index: 4000;
            animation: slideIn 0.3s ease;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(100px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .notification.show {
            display: flex;
        }

        /* Responsive */
        @media (max-width: 1024px) {
            .modal-body {
                flex-direction: column;
            }
        }

        @media (max-width: 768px) {
            .header-content {
                flex-wrap: wrap;
            }
            
            .search-bar {
                order: 3;
                width: 100%;
            }
            
            .hero-slide {
                flex-direction: column;
                text-align: center;
            }
            
            .hero-content {
                padding: 20px;
            }
            
            .products-grid {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            }
            
            .cart-sidebar {
                max-width: 100%;
            }
        }

        @media (max-width: 480px) {
            .products-grid {
                grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            }
            
            .modal-body {
                padding: 20px;
            }
            
            .modal-actions {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Login Page -->
    <div class="login-page" id="loginPage">
        <div class="login-card">
            <div class="brand-logo">
                <i class="fas fa-shopping-cart"></i>
            </div>
            <h1 class="brand-name">MD Cart<span class="plus">+</span></h1>
            <p class="tagline">India's Most Loved Shopping Platform</p>
            
            <div class="login-form">
                <input type="email" id="email" placeholder="Enter Email ID" required>
                <input type="password" id="password" placeholder="Enter Password" required>
                <button class="login-btn" onclick="login()">
                    <i class="fas fa-sign-in-alt"></i> Login
                </button>
                
                <div class="or-divider">OR</div>
                
                <button class="signup-btn" onclick="showSignup()">
                    <i class="fas fa-user-plus"></i> Create Account
                </button>
                
                <button class="guest-btn" onclick="continueAsGuest()">
                    <i class="fas fa-shopping-bag"></i> Continue as Guest
                </button>
            </div>
        </div>
    </div>

    <!-- Main Store -->
    <div class="main-store" id="mainStore">
        <!-- Top Bar -->
        <div class="top-bar">
            <div class="container top-bar-content">
                <div class="top-links">
                    <a href="#"><i class="fas fa-mobile-alt"></i> Download App</a>
                    <a href="#"><i class="fas fa-map-marker-alt"></i> Select Location</a>
                    <a href="#"><i class="fas fa-question-circle"></i> 24x7 Customer Care</a>
                </div>
                <div class="top-links">
                    <a href="#" onclick="showProfile()"><i class="fas fa-user"></i> Profile</a>
                    <a href="#" onclick="showOrders()"><i class="fas fa-box"></i> Orders</a>
                    <a href="#" onclick="showWishlist()"><i class="fas fa-heart"></i> Wishlist</a>
                </div>
            </div>
        </div>

        <!-- Header -->
        <header class="main-header">
            <div class="container header-content">
                <a href="#" class="logo" onclick="showHome()">
                    <div class="logo-icon">
                        <i class="fas fa-shopping-cart"></i>
                    </div>
                    <div class="logo-text">MD<span>CART</span></div>
                </a>

                <div class="search-bar">
                    <input type="text" class="search-input" placeholder="Search for products, brands and more">
                    <button class="search-btn">
                        <i class="fas fa-search"></i>
                    </button>
                </div>

                <div class="header-actions">
                    <div class="user-menu">
                        <div class="user-avatar" onclick="toggleUserMenu()">
                            <i class="fas fa-user"></i>
                        </div>
                    </div>
                    
                    <a href="#" class="action-item" onclick="showWishlist()">
                        <i class="fas fa-heart action-icon"></i>
                        Wishlist
                    </a>
                    
                    <a href="#" class="action-item" onclick="toggleCart()" style="position: relative;">
                        <i class="fas fa-shopping-cart action-icon"></i>
                        Cart
                        <span class="cart-count" id="cartCount">0</span>
                    </a>
                </div>
            </div>
        </header>

        <!-- Categories Bar -->
        <nav class="categories-bar">
            <div class="container">
                <div class="categories">
                    <a href="#" class="category-item" onclick="filterCategory('electronics')">
                        <div class="category-icon">
                            <i class="fas fa-tv"></i>
                        </div>
                        Electronics
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('fashion')">
                        <div class="category-icon">
                            <i class="fas fa-tshirt"></i>
                        </div>
                        Fashion
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('mobiles')">
                        <div class="category-icon">
                            <i class="fas fa-mobile-alt"></i>
                        </div>
                        Mobiles
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('home')">
                        <div class="category-icon">
                            <i class="fas fa-home"></i>
                        </div>
                        Home
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('appliances')">
                        <div class="category-icon">
                            <i class="fas fa-blender"></i>
                        </div>
                        Appliances
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('beauty')">
                        <div class="category-icon">
                            <i class="fas fa-spa"></i>
                        </div>
                        Beauty
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('toys')">
                        <div class="category-icon">
                            <i class="fas fa-gamepad"></i>
                        </div>
                        Toys & Games
                    </a>
                    
                    <a href="#" class="category-item" onclick="filterCategory('grocery')">
                        <div class="category-icon">
                            <i class="fas fa-shopping-basket"></i>
                        </div>
                        Grocery
                    </a>
                </div>
            </div>
        </nav>

        <!-- Hero Banner -->
        <section class="hero-section">
            <div class="container">
                <div class="hero-slider">
                    <div class="hero-slide">
                        <div class="hero-content">
                            <h2 class="hero-title">Big Billion Days Sale!</h2>
                            <p class="hero-subtitle">Up to 70% Off on Top Brands. Limited Time Offer</p>
                            <button class="btn btn-secondary" onclick="showAllDeals()">
                                <i class="fas fa-bolt"></i> Shop Now
                            </button>
                        </div>
                        <div class="hero-image">
                            <div style="font-size: 120px; color: white;">
                                🎁
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Deals of the Day -->
        <section class="products-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">
                        <i class="fas fa-bolt" style="color: #ff9f00;"></i>
                        Deals of the Day
                    </h2>
                    <a href="#" class="view-all" onclick="showAllDeals()">View All</a>
                </div>
                <div class="products-grid" id="dealsGrid">
                    <!-- Deals will be loaded here -->
                </div>
            </div>
        </section>

        <!-- Top Products -->
        <section class="products-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">
                        <i class="fas fa-fire" style="color: #ff6b6b;"></i>
                        Best Selling Products
                    </h2>
                    <a href="#" class="view-all" onclick="showAllProducts()">View All</a>
                </div>
                <div class="products-grid" id="productsGrid">
                    <!-- Products will be loaded here -->
                </div>
            </div>
        </section>

        <!-- Categories Sections -->
        <section class="products-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">
                        <i class="fas fa-mobile-alt" style="color: #2874f0;"></i>
                        Top Mobiles
                    </h2>
                    <a href="#" class="view-all" onclick="filterCategory('mobiles')">View All</a>
                </div>
                <div class="products-grid" id="mobilesGrid">
                    <!-- Mobiles will be loaded here -->
                </div>
            </div>
        </section>

        <section class="products-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">
                        <i class="fas fa-laptop" style="color: #00d2d3;"></i>
                        Laptops & Computers
                    </h2>
                    <a href="#" class="view-all" onclick="filterCategory('electronics')">View All</a>
                </div>
                <div class="products-grid" id="laptopsGrid">
                    <!-- Laptops will be loaded here -->
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="main-footer">
            <div class="container">
                <div class="footer-content">
                    <div class="footer-section">
                        <h3>About MD Cart</h3>
                        <ul class="footer-links">
                            <li><a href="#">Contact Us</a></li>
                            <li><a href="#">About Us</a></li>
                            <li><a href="#">Careers</a></li>
                            <li><a href="#">Press</a></li>
                            <li><a href="#">Corporate Information</a></li>
                        </ul>
                    </div>
                    
                    <div class="footer-section">
                        <h3>Help</h3>
                        <ul class="footer-links">
                            <li><a href="#">Payments</a></li>
                            <li><a href="#">Shipping</a></li>
                            <li><a href="#">Cancellation & Returns</a></li>
                            <li><a href="#">FAQ</a></li>
                            <li><a href="#">Report Infringement</a></li>
                        </ul>
                    </div>
                    
                    <div class="footer-section">
                        <h3>Policy</h3>
                        <ul class="footer-links">
                            <li><a href="#">Return Policy</a></li>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Security</a></li>
                            <li><a href="#">Privacy</a></li>
                            <li><a href="#">Sitemap</a></li>
                        </ul>
                    </div>
                    
                    <div class="footer-section">
                        <h3>Social</h3>
                        <div class="social-links">
                            <a href="#"><i class="fab fa-facebook"></i></a>
                            <a href="#"><i class="fab fa-twitter"></i></a>
                            <a href="#"><i class="fab fa-instagram"></i></a>
                            <a href="#"><i class="fab fa-youtube"></i></a>
                        </div>
                    </div>
                </div>
                
                <div class="footer-bottom">
                    <div>© 2024 MD Cart. All rights reserved.</div>
                    <div>Made with ❤️ in India</div>
                </div>
            </div>
        </footer>
    </div>

    <!-- Cart Sidebar -->
    <div class="cart-overlay" id="cartOverlay" onclick="toggleCart()"></div>
    <div class="cart-sidebar" id="cartSidebar">
        <div class="cart-header">
            <h2 class="cart-title">Shopping Cart</h2>
            <button class="close-cart" onclick="toggleCart()">
                <i class="fas fa-times"></i>
            </button>
        </div>
        <div class="cart-items" id="cartItems">
            <!-- Cart items will be loaded here -->
        </div>
        <div class="cart-footer">
            <div class="cart-summary" id="cartSummary">
                <!-- Summary will be loaded here -->
            </div>
            <button class="checkout-btn" onclick="checkout()">
                <i class="fas fa-lock"></i> Proceed to Checkout
            </button>
        </div>
    </div>

    <!-- Product Modal -->
    <div class="product-modal" id="productModal">
        <div class="modal-content">
            <button class="modal-close" onclick="closeProductModal()">
                <i class="fas fa-times"></i>
            </button>
            <div class="modal-body" id="modalBody">
                <!-- Product details will be loaded here -->
            </div>
        </div>
    </div>

    <!-- Notification -->
    <div class="notification" id="notification">
        <i class="fas fa-check-circle"></i>
        <span id="notificationText"></span>
    </div>

    <script>
        // Product Database - Real E-commerce Products
        const products = {
            deals: [
                {
                    id: 1,
                    name: "Apple iPhone 14 Pro Max",
                    brand: "Apple",
                    price: 129999,
                    originalPrice: 139999,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.8,
                    reviews: 12450,
                    discount: 7,
                    description: "6.7-inch Super Retina XDR display, A16 Bionic chip, 48MP Main camera, Face ID",
                    specs: ["256GB Storage", "Dynamic Island", "Always-On display", "Emergency SOS"],
                    offers: ["Bank Offer: 10% Instant Discount", "No Cost EMI", "Exchange Offer: Up to ₹15,000"]
                },
                {
                    id: 2,
                    name: "Samsung Galaxy S23 Ultra",
                    brand: "Samsung",
                    price: 124999,
                    originalPrice: 134999,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.7,
                    reviews: 8940,
                    discount: 7,
                    description: "6.8-inch Dynamic AMOLED 2X, Snapdragon 8 Gen 2, 200MP camera, S Pen included",
                    specs: ["512GB Storage", "12GB RAM", "5000mAh Battery", "45W Fast Charging"],
                    offers: ["Free Galaxy Buds2 Pro", "No Cost EMI", "Extra ₹8000 Exchange Bonus"]
                },
                {
                    id: 3,
                    name: "OnePlus 11 5G",
                    brand: "OnePlus",
                    price: 56999,
                    originalPrice: 61999,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.6,
                    reviews: 5670,
                    discount: 8,
                    description: "6.7-inch Fluid AMOLED, Snapdragon 8 Gen 2, Hasselblad camera, 100W charging",
                    specs: ["256GB Storage", "16GB RAM", "5000mAh Battery", "Dolby Atmos"],
                    offers: ["Instant Discount: ₹3000", "No Cost EMI", "Free OnePlus Buds Z2"]
                },
                {
                    id: 4,
                    name: "MacBook Air M2",
                    brand: "Apple",
                    price: 114990,
                    originalPrice: 119900,
                    image: "💻",
                    category: "electronics",
                    rating: 4.9,
                    reviews: 3240,
                    discount: 4,
                    description: "13.6-inch Liquid Retina display, M2 chip, 8GB RAM, 256GB SSD, up to 18 hours battery",
                    specs: ["8-core CPU", "10-core GPU", "MagSafe charging", "Touch ID"],
                    offers: ["Bank Offer: 10% Instant Discount", "No Cost EMI", "Free AirPods"]
                }
            ],
            mobiles: [
                {
                    id: 5,
                    name: "Google Pixel 7 Pro",
                    brand: "Google",
                    price: 84999,
                    originalPrice: 89999,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.5,
                    reviews: 2340,
                    discount: 6,
                    description: "6.7-inch QHD+ LTPO OLED, Google Tensor G2, 50MP main camera, 30x Super Res Zoom",
                    specs: ["128GB Storage", "12GB RAM", "5000mAh Battery", "Wireless Charging"],
                    offers: ["Instant Discount: ₹5000", "No Cost EMI", "Free Pixel Buds A-Series"]
                },
                {
                    id: 6,
                    name: "Xiaomi 13 Pro",
                    brand: "Xiaomi",
                    price: 79999,
                    originalPrice: 84999,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.4,
                    reviews: 1890,
                    discount: 6,
                    description: "6.73-inch AMOLED, Snapdragon 8 Gen 2, Leica camera, 120W HyperCharge",
                    specs: ["256GB Storage", "12GB RAM", "4820mAh Battery", "Dolby Vision"],
                    offers: ["Bank Offer: 10% Instant Discount", "No Cost EMI", "Free Mi Watch"]
                },
                {
                    id: 7,
                    name: "Nothing Phone (2)",
                    brand: "Nothing",
                    price: 44999,
                    originalPrice: 49999,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.3,
                    reviews: 4560,
                    discount: 10,
                    description: "6.7-inch LTPO OLED, Snapdragon 8+ Gen 1, Glyph Interface, 50MP dual camera",
                    specs: ["256GB Storage", "12GB RAM", "4700mAh Battery", "45W Fast Charging"],
                    offers: ["Instant Discount: ₹4000", "No Cost EMI", "Exchange Bonus: ₹5000"]
                },
                {
                    id: 8,
                    name: "Vivo X90 Pro",
                    brand: "Vivo",
                    price: 84990,
                    originalPrice: 89990,
                    image: "📱",
                    category: "mobiles",
                    rating: 4.6,
                    reviews: 1230,
                    discount: 6,
                    description: "6.78-inch AMOLED, MediaTek Dimensity 9200, ZEISS camera, 120W FlashCharge",
                    specs: ["256GB Storage", "12GB RAM", "4870mAh Battery", "IP68 Water Resistant"],
                    offers: ["Bank Offer: 10% Instant Discount", "No Cost EMI", "Free Vivo TWS Earphone"]
                }
            ],
            electronics: [
                {
                    id: 9,
                    name: "Dell XPS 13 Plus",
                    brand: "Dell",
                    price: 149990,
                    originalPrice: 164990,
                    image: "💻",
                    category: "electronics",
                    rating: 4.7,
                    reviews: 890,
                    discount: 9,
                    description: "13.4-inch OLED Touch, Intel Core i7, 16GB RAM, 1TB SSD, Windows 11 Pro",
                    specs: ["Intel Iris Xe Graphics", "4K OLED Display", "Thunderbolt 4", "FHD Webcam"],
                    offers: ["Instant Discount: ₹15,000", "No Cost EMI", "Free Microsoft Office"]
                },
                {
                    id: 10,
                    name: "Samsung Odyssey G9",
                    brand: "Samsung",
                    price: 134999,
                    originalPrice: 149999,
                    image: "🖥️",
                    category: "electronics",
                    rating: 4.8,
                    reviews: 670,
                    discount: 10,
                    description: "49-inch Dual QHD Curved Gaming Monitor, 240Hz, 1ms, QLED, G-Sync Compatible",
                    specs: ["5120x1440 Resolution", "1000R Curvature", "HDR1000", "DisplayPort 1.4"],
                    offers: ["No Cost EMI", "Exchange Offer", "Extra Warranty"]
                },
                {
                    id: 11,
                    name: "Sony WH-1000XM5",
                    brand: "Sony",
                    price: 29990,
                    originalPrice: 34990,
                    image: "🎧",
                    category: "electronics",
                    rating: 4.9,
                    reviews: 4560,
                    discount: 14,
                    description: "Industry-leading noise cancellation, 30-hour battery, Multipoint connection",
                    specs: ["8 Mics for Call Quality", "Quick Charging", "LDAC Support", "Auto NC Optimizer"],
                    offers: ["Instant Discount: ₹4000", "No Cost EMI", "Free Carry Case"]
                },
                {
                    id: 12,
                    name: "Apple Watch Series 8",
                    brand: "Apple",
                    price: 45900,
                    originalPrice: 49900,
                    image: "⌚",
                    category: "electronics",
                    rating: 4.7,
                    reviews: 3450,
                    discount: 8,
                    description: "45mm GPS + Cellular, Always-On Retina display, Temperature sensing, Crash Detection",
                    specs: ["Blood Oxygen App", "ECG App", "Water Resistant 50m", "Fast Charging"],
                    offers: ["Bank Offer: 10% Instant Discount", "No Cost EMI", "Free Apple Care+"]
                }
            ],
            fashion: [
                {
                    id: 13,
                    name: "Nike Air Max 270",
                    brand: "Nike",
                    price: 10995,
                    originalPrice: 12995,
                    image: "👟",
                    category: "fashion",
                    rating: 4.5,
                    reviews: 2340,
                    discount: 15,
                    description: "Men's Running Shoes with largest Air unit for all-day comfort",
                    specs: ["Breathable Mesh", "Rubber Outsole", "Max Air Cushioning", "Lightweight Design"],
                    offers: ["Bank Offer: 10% Instant Discount", "No Cost EMI", "Extra 10% Off"]
                },
                {
                    id: 14,
                    name: "Levi's 501 Original Fit",
                    brand: "Levi's",
                    price: 3999,
                    originalPrice: 4999,
                    image: "👖",
                    category: "fashion",
                    rating: 4.6,
                    reviews: 1890,
                    discount: 20,
                    description: "Men's Jeans - Original fit, button fly, straight leg",
                    specs: ["100% Cotton", "Regular Fit", "Button Fly", "Five Pockets"],
                    offers: ["Buy 1 Get 1 Free", "Extra 20% Off", "No Cost EMI"]
                }
            ],
            home: [
                {
                    id: 15,
                    name: "Philips Hue Starter Kit",
                    brand: "Philips",
                    price: 14999,
                    originalPrice: 17999,
                    image: "💡",
                    category: "home",
                    rating: 4.7,
                    reviews: 890,
                    discount: 17,
                    description: "Smart LED light bulbs with bridge, works with Alexa, Google Assistant",
                    specs: ["16 Million Colors", "Voice Control", "Automation", "Energy Saving"],
                    offers: ["Instant Discount: ₹2000", "No Cost EMI", "Free Smart Plug"]
                }
            ],
            appliances: [
                {
                    id: 16,
                    name: "Samsung 8kg Front Load",
                    brand: "Samsung",
                    price: 35990,
                    originalPrice: 42990,
                    image: "🧺",
                    category: "appliances",
                    rating: 4.6,
                    reviews: 1560,
                    discount: 16,
                    description: "AI Control Washing Machine with Eco Bubble technology, Digital Inverter",
                    specs: ["1400 RPM", "Steam Wash", "Quick Wash", "Baby Care"],
                    offers: ["Exchange Bonus: ₹5000", "No Cost EMI", "Extra Warranty"]
                }
            ]
        };

        // Cart and User Data
        let cart = [];
        let currentUser = null;
        let wishlist = [];

        // DOM Elements
        const loginPage = document.getElementById('loginPage');
        const mainStore = document.getElementById('mainStore');
        const cartSidebar = document.getElementById('cartSidebar');
        const cartOverlay = document.getElementById('cartOverlay');
        const productModal = document.getElementById('productModal');
        const notification = document.getElementById('notification');

        // Initialize
        function init() {
            renderDeals();
            renderProducts();
            renderMobiles();
            renderLaptops();
            updateCartCount();
        }

        // Authentication
        function login() {
            const email = document.getElementById('email').value;
            const password = document.getElementById('password').value;
            
            if (!email || !password) {
                showNotification('Please enter email and password');
                return;
            }
            
            currentUser = {
                name: email.split('@')[0],
                email: email
            };
            
            showNotification('Login successful!');
            showMainStore();
        }

        function showSignup() {
            showNotification('Redirecting to signup page...');
        }

        function continueAsGuest() {
            currentUser = null;
            showMainStore();
        }

        function showMainStore() {
            loginPage.style.display = 'none';
            mainStore.style.display = 'block';
            init();
        }

        function logout() {
            currentUser = null;
            showNotification('Logged out successfully');
            mainStore.style.display = 'none';
            loginPage.style.display = 'flex';
        }

        // Product Rendering
        function renderDeals() {
            const grid = document.getElementById('dealsGrid');
            grid.innerHTML = '';
            
            products.deals.forEach(product => {
                grid.appendChild(createProductCard(product));
            });
        }

        function renderProducts() {
            const grid = document.getElementById('productsGrid');
            grid.innerHTML = '';
            
            // Combine products from different categories
            const allProducts = [
                ...products.mobiles,
                ...products.electronics,
                ...products.fashion,
                ...products.home,
                ...products.appliances
            ];
            
            // Take first 8 products
            allProducts.slice(0, 8).forEach(product => {
                grid.appendChild(createProductCard(product));
            });
        }

        function renderMobiles() {
            const grid = document.getElementById('mobilesGrid');
            grid.innerHTML = '';
            
            products.mobiles.forEach(product => {
                grid.appendChild(createProductCard(product));
            });
        }

        function renderLaptops() {
            const grid = document.getElementById('laptopsGrid');
            grid.innerHTML = '';
            
            products.electronics.forEach(product => {
                grid.appendChild(createProductCard(product));
            });
        }

        function createProductCard(product) {
            const card = document.createElement('div');
            card.className = 'product-card';
            card.innerHTML = `
                <div class="product-badge">${product.discount}% OFF</div>
                <div class="product-image">
                    <div style="font-size: 60px;">${product.image}</div>
                    <button class="wishlist-btn" onclick="toggleWishlist(${product.id})">
                        <i class="far fa-heart"></i>
                    </button>
                </div>
                <div class="product-details">
                    <div class="product-brand">${product.brand}</div>
                    <div class="product-title">${product.name}</div>
                    <div class="product-rating">
                        <div class="rating-stars">
                            ${'★'.repeat(Math.floor(product.rating))}${'☆'.repeat(5-Math.floor(product.rating))}
                        </div>
                        <div class="rating-count">(${product.reviews.toLocaleString()})</div>
                    </div>
                    <div class="price-section">
                        <div class="current-price">₹${product.price.toLocaleString()}</div>
                        <div class="original-price">₹${product.originalPrice.toLocaleString()}</div>
                        <div class="discount">${product.discount}% off</div>
                    </div>
                    <button class="add-to-cart" onclick="addToCart(${product.id})">
                        <i class="fas fa-shopping-cart"></i> ADD TO CART
                    </button>
                    <button class="buy-now" onclick="buyNow(${product.id})">
                        <i class="fas fa-bolt"></i> BUY NOW
                    </button>
                </div>
            `;
            
            // Add click event for product details
            card.addEventListener('click', (e) => {
                if (!e.target.closest('button')) {
                    showProductDetails(product.id);
                }
            });
            
            return card;
        }

        // Product Details Modal
        function showProductDetails(productId) {
            const product = findProductById(productId);
            if (!product) return;
            
            const modalBody = document.getElementById('modalBody');
            modalBody.innerHTML = `
                <div class="modal-images">
                    <div class="main-image">
                        <div style="font-size: 120px;">${product.image}</div>
                    </div>
                </div>
                <div class="modal-details">
                    <h1 class="modal-title">${product.name}</h1>
                    <div class="modal-rating">
                        <div class="rating-stars" style="font-size: 18px;">
                            ${'★'.repeat(Math.floor(product.rating))}${'☆'.repeat(5-Math.floor(product.rating))}
                        </div>
                        <div class="rating-count" style="font-size: 14px;">${product.rating} (${product.reviews.toLocaleString()} ratings)</div>
                    </div>
                    <div class="modal-price">₹${product.price.toLocaleString()}</div>
                    <div style="margin-bottom: 20px;">
                        <span style="color: #878787; text-decoration: line-through; margin-right: 10px;">
                            ₹${product.originalPrice.toLocaleString()}
                        </span>
                        <span style="color: #388e3c; font-weight: 600;">
                            ${product.discount}% off
                        </span>
                    </div>
                    
                    <div class="modal-offers">
                        <h3 style="margin-bottom: 10px; font-size: 16px;">Available Offers</h3>
                        ${product.offers.map(offer => `
                            <div class="offer-item">
                                <i class="fas fa-tag" style="color: #388e3c;"></i>
                                <span>${offer}</span>
                            </div>
                        `).join('')}
                    </div>
                    
                    <div class="modal-specs">
                        <h3 style="margin-bottom: 10px; font-size: 16px;">Specifications</h3>
                        ${product.specs.map(spec => `
                            <div class="spec-item">
                                <div class="spec-label">•</div>
                                <div class="spec-value">${spec}</div>
                            </div>
                        `).join('')}
                    </div>
                    
                    <div style="margin: 20px 0; padding: 15px; background: #f5f5f5; border-radius: 4px;">
                        <div style="font-weight: 600; margin-bottom: 5px;">Description</div>
                        <div style="color: #666;">${product.description}</div>
                    </div>
                    
                    <div class="modal-actions">
                        <button class="btn btn-primary" style="flex: 2;" onclick="addToCart(${product.id}); closeProductModal();">
                            <i class="fas fa-shopping-cart"></i> ADD TO CART
                        </button>
                        <button class="btn btn-secondary" style="flex: 1;" onclick="buyNow(${product.id}); closeProductModal();">
                            <i class="fas fa-bolt"></i> BUY NOW
                        </button>
                    </div>
                </div>
            `;
            
            productModal.classList.add('active');
        }

        function closeProductModal() {
            productModal.classList.remove('active');
        }

        // Cart Functions
        function addToCart(productId) {
            const product = findProductById(productId);
            if (!product) return;
            
            const existingItem = cart.find(item => item.id === productId);
            
            if (existingItem) {
                existingItem.quantity += 1;
            } else {
                cart.push({
                    ...product,
                    quantity: 1
                });
            }
            
            updateCartCount();
            if (cartSidebar.classList.contains('active')) {
                renderCart();
            }
            
            showNotification(`${product.name} added to cart!`);
        }

        function removeFromCart(productId) {
            cart = cart.filter(item => item.id !== productId);
            updateCartCount();
            renderCart();
            showNotification('Item removed from cart');
        }

        function updateQuantity(productId, change) {
            const item = cart.find(item => item.id === productId);
            if (item) {
                item.quantity += change;
                if (item.quantity < 1) {
                    removeFromCart(productId);
                } else {
                    updateCartCount();
                    renderCart();
                }
            }
        }

        function updateCartCount() {
            const totalItems = cart.reduce((total, item) => total + item.quantity, 0);
            document.getElementById('cartCount').textContent = totalItems;
        }

        function renderCart() {
            const cartItems = document.getElementById('cartItems');
            const cartSummary = document.getElementById('cartSummary');
            
            if (cart.length === 0) {
                cartItems.innerHTML = `
                    <div class="empty-cart">
                        <i class="fas fa-shopping-cart"></i>
                        <h3 style="margin-bottom: 10px;">Your cart is empty</h3>
                        <p>Add items to get started!</p>
                        <button class="btn btn-primary" style="margin-top: 20px;" onclick="toggleCart(); showHome()">
                            <i class="fas fa-shopping-bag"></i> Continue Shopping
                        </button>
                    </div>
                `;
                cartSummary.innerHTML = '';
                return;
            }
            
            let subtotal = 0;
            let discount = 0;
            
            cartItems.innerHTML = cart.map(item => {
                const itemTotal = item.price * item.quantity;
                subtotal += itemTotal;
                discount += (item.originalPrice - item.price) * item.quantity;
                
                return `
                    <div class="cart-item">
                        <div class="cart-item-image">
                            <div style="font-size: 40px;">${item.image}</div>
                        </div>
                        <div class="cart-item-details">
                            <div class="cart-item-title">${item.name}</div>
                            <div class="cart-item-price">₹${item.price.toLocaleString()}</div>
                            <div class="cart-item-actions">
                                <button class="quantity-btn" onclick="updateQuantity(${item.id}, -1)">
                                    <i class="fas fa-minus"></i>
                                </button>
                                <span class="quantity">${item.quantity}</span>
                                <button class="quantity-btn" onclick="updateQuantity(${item.id}, 1)">
                                    <i class="fas fa-plus"></i>
                                </button>
                                <button class="remove-item" onclick="removeFromCart(${item.id})">
                                    Remove
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            }).join('');
            
            const delivery = 0; // Free delivery
            const total = subtotal - discount + delivery;
            
            cartSummary.innerHTML = `
                <div class="summary-row">
                    <span>Subtotal</span>
                    <span>₹${subtotal.toLocaleString()}</span>
                </div>
                <div class="summary-row">
                    <span>Discount</span>
                    <span style="color: #388e3c;">-₹${discount.toLocaleString()}</span>
                </div>
                <div class="summary-row">
                    <span>Delivery</span>
                    <span>${delivery === 0 ? 'FREE' : '₹' + delivery}</span>
                </div>
                <div class="summary-row total">
                    <span>Total</span>
                    <span>₹${total.toLocaleString()}</span>
                </div>
            `;
        }

        function toggleCart() {
            if (cartSidebar.classList.contains('active')) {
                cartSidebar.classList.remove('active');
                cartOverlay.classList.remove('active');
            } else {
                cartSidebar.classList.add('active');
                cartOverlay.classList.add('active');
                renderCart();
            }
        }

        // Helper Functions
        function findProductById(id) {
            for (const category in products) {
                const product = products[category].find(p => p.id === id);
                if (product) return product;
            }
            return null;
        }

        function showNotification(message) {
            document.getElementById('notificationText').textContent = message;
            notification.classList.add('show');
            setTimeout(() => {
                notification.classList.remove('show');
            }, 3000);
        }

        function toggleWishlist(productId) {
            const product = findProductById(productId);
            if (!product) return;
            
            const index = wishlist.findIndex(item => item.id === productId);
            if (index === -1) {
                wishlist.push(product);
                showNotification('Added to wishlist');
            } else {
                wishlist.splice(index, 1);
                showNotification('Removed from wishlist');
            }
        }

        function buyNow(productId) {
            addToCart(productId);
            toggleCart();
        }

        function checkout() {
            if (cart.length === 0) {
                showNotification('Your cart is empty');
                return;
            }
            
            if (!currentUser) {
                showNotification('Please login to checkout');
                return;
            }
            
            showNotification(`Order placed successfully! Total: ₹${cart.reduce((total, item) => total + (item.price * item.quantity), 0).toLocaleString()}`);
            cart = [];
            updateCartCount();
            toggleCart();
        }

        // Navigation Functions
        function showHome() {
            window.scrollTo(0, 0);
        }

        function showProfile() {
            if (currentUser) {
                showNotification(`Welcome ${currentUser.name}!`);
            } else {
                showNotification('Please login to view profile');
            }
        }

        function showOrders() {
            showNotification('Your orders will appear here');
        }

        function showWishlist() {
            if (wishlist.length === 0) {
                showNotification('Your wishlist is empty');
            } else {
                showNotification(`You have ${wishlist.length} items in wishlist`);
            }
        }

        function filterCategory(category) {
            showNotification(`Showing ${category} products`);
            // In a real app, this would filter products
        }

        function showAllDeals() {
            showNotification('Showing all deals');
        }

        function showAllProducts() {
            showNotification('Showing all products');
        }

        function toggleUserMenu() {
            if (currentUser) {
                const choice = confirm('Do you want to logout?');
                if (choice) {
                    logout();
                }
            } else {
                showNotification('Please login first');
            }
        }

        // Close modal when clicking outside
        productModal.addEventListener('click', (e) => {
            if (e.target === productModal) {
                closeProductModal();
            }
        });

        // Initialize when page loads
        window.onload = function() {
            loginPage.style.display = 'flex';
            mainStore.style.display = 'none';
        };
    </script>
</body>
</html>
