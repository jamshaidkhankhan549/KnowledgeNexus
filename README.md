<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Knowledge Nexus | Scribd - Document Sharing Hub</title>
    <meta name="description" content="Share and discover documents, presentations, and research across University, School, College, and specialized Law fields.">
    <!-- Link to Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Link to Google Adsense (ca-app-pub-8123763654650570~3731172424) -->
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-app-pub-8123763654650570~3731172424" crossorigin="anonymous"></script>
    <style>
        /* ===== CSS Reset & Base Styles ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        a {
            text-decoration: none;
            color: inherit;
        }
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        .btn {
            display: inline-block;
            padding: 10px 24px;
            background-color: #4361ee;
            color: white;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: background-color 0.3s ease;
        }
        .btn:hover {
            background-color: #3a56d4;
        }
        .btn-secondary {
            background-color: #6c757d;
        }
        .btn-secondary:hover {
            background-color: #5a6268;
        }
        .hidden {
            display: none !important;
        }
        /* ===== Header & Navigation ===== */
        header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            display: flex;
            align-items: center;
        }
        .logo i {
            margin-right: 10px;
            color: #4cc9f0;
        }
        .logo span {
            color: #4cc9f0;
        }
        nav ul {
            display: flex;
            list-style: none;
        }
        nav ul li {
            margin-left: 2rem;
        }
        nav ul li a {
            font-weight: 600;
            font-size: 1rem;
            padding: 8px 0;
            position: relative;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #4cc9f0;
        }
        nav ul li a.active {
            color: #4cc9f0;
        }
        nav ul li a.active::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 3px;
            background-color: #4cc9f0;
            border-radius: 2px;
        }
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        /* ===== Hero Section ===== */
        .hero {
            padding: 4rem 0;
            text-align: center;
            background-color: #fff;
            border-bottom: 1px solid #eee;
        }
        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 1rem;
            color: #1e3c72;
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
            color: #555;
        }
        .search-bar {
            max-width: 600px;
            margin: 2rem auto 0;
            display: flex;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            border-radius: 50px;
            overflow: hidden;
        }
        .search-bar input {
            flex-grow: 1;
            padding: 18px 24px;
            border: none;
            font-size: 1rem;
            outline: none;
        }
        .search-bar button {
            padding: 0 30px;
            background-color: #4361ee;
            color: white;
            border: none;
            cursor: pointer;
            font-size: 1.1rem;
            transition: background-color 0.3s;
        }
        .search-bar button:hover {
            background-color: #3a56d4;
        }
        /* ===== Main Content & Layout ===== */
        .main-content {
            display: flex;
            padding: 2rem 0;
            gap: 2rem;
        }
        .sidebar {
            flex: 0 0 250px;
            background-color: white;
            border-radius: 12px;
            padding: 1.5rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            height: fit-content;
        }
        .sidebar h3 {
            margin-bottom: 1rem;
            padding-bottom: 0.75rem;
            border-bottom: 2px solid #4361ee;
            color: #1e3c72;
        }
        .category-list {
            list-style: none;
        }
        .category-list li {
            margin-bottom: 0.75rem;
        }
        .category-list li a {
            display: block;
            padding: 10px 15px;
            border-radius: 8px;
            transition: all 0.3s;
            color: #444;
            font-weight: 500;
        }
        .category-list li a:hover,
        .category-list li a.active {
            background-color: #eef2ff;
            color: #4361ee;
            padding-left: 20px;
        }
        .subcategory-list {
            list-style: none;
            margin-top: 0.5rem;
            margin-left: 1.5rem;
            border-left: 2px dashed #ddd;
            padding-left: 1rem;
            display: none;
        }
        .category-list li.active .subcategory-list {
            display: block;
        }
        .subcategory-list li a {
            padding: 8px 12px;
            font-size: 0.9rem;
            color: #666;
        }
        .subcategory-list li a:hover {
            color: #3a56d4;
            background-color: transparent;
            padding-left: 15px;
        }
        .content-area {
            flex: 1;
        }
        /* ===== Ad Placeholder & Document List ===== */
        .ad-placeholder {
            background-color: #f8f9fa;
            border: 2px dashed #adb5bd;
            border-radius: 8px;
            padding: 2rem;
            text-align: center;
            margin-bottom: 2rem;
            color: #6c757d;
            font-style: italic;
        }
        .ad-placeholder i {
            font-size: 2rem;
            margin-bottom: 1rem;
            color: #adb5bd;
        }
        .section-title {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
            padding-bottom: 0.75rem;
            border-bottom: 1px solid #dee2e6;
        }
        .section-title h2 {
            color: #1e3c72;
        }
        .documents-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        .document-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .document-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        .doc-thumbnail {
            height: 180px;
            background-color: #e9ecef;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #4361ee;
            font-size: 3rem;
        }
        .doc-info {
            padding: 1.5rem;
        }
        .doc-info h4 {
            margin-bottom: 0.5rem;
            color: #212529;
        }
        .doc-info p {
            color: #6c757d;
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }
        .doc-meta {
            display: flex;
            justify-content: space-between;
            font-size: 0.8rem;
            color: #adb5bd;
        }
        /* ===== Upload Modal ===== */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(0, 0, 0, 0.7);
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 2000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }
        .modal-overlay.active {
            opacity: 1;
            visibility: visible;
        }
        .upload-modal {
            background: white;
            width: 90%;
            max-width: 600px;
            border-radius: 16px;
            padding: 2rem;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            transform: scale(0.9);
            transition: transform 0.3s ease;
        }
        .modal-overlay.active .upload-modal {
            transform: scale(1);
        }
        .upload-modal h3 {
            color: #1e3c72;
            margin-bottom: 1.5rem;
            padding-bottom: 1rem;
            border-bottom: 1px solid #eee;
        }
        .form-group {
            margin-bottom: 1.5rem;
        }
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #495057;
        }
        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px 16px;
            border: 1px solid #ced4da;
            border-radius: 8px;
            font-size: 1rem;
            transition: border-color 0.3s;
        }
        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            border-color: #4361ee;
            outline: none;
        }
        .file-upload-area {
            border: 3px dashed #adb5bd;
            border-radius: 12px;
            padding: 3rem 2rem;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            background-color: #f8f9fa;
        }
        .file-upload-area:hover,
        .file-upload-area.dragover {
            border-color: #4361ee;
            background-color: #eef2ff;
        }
        .file-upload-area i {
            font-size: 3rem;
            color: #6c757d;
            margin-bottom: 1rem;
        }
        .file-upload-area p {
            color: #6c757d;
        }
        .modal-actions {
            display: flex;
            justify-content: flex-end;
            gap: 1rem;
            margin-top: 2rem;
        }
        /* ===== Footer & SEO ===== */
        footer {
            background-color: #1a202c;
            color: #cbd5e0;
            padding: 3rem 0 2rem;
            margin-top: 3rem;
        }
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }
        .footer-column h4 {
            color: white;
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
        }
        .footer-links {
            list-style: none;
        }
        .footer-links li {
            margin-bottom: 0.75rem;
        }
        .footer-links a {
            color: #a0aec0;
            transition: color 0.3s;
        }
        .footer-links a:hover {
            color: #4cc9f0;
        }
        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #2d3748;
            color: #a0aec0;
            font-size: 0.9rem;
        }
        /* ===== Responsive Design ===== */
        @media (max-width: 992px) {
            .main-content {
                flex-direction: column;
            }
            .sidebar {
                flex: none;
                width: 100%;
            }
            .documents-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }
        }
        @media (max-width: 768px) {
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: #1e3c72;
                flex-direction: column;
                padding: 1rem 0;
                box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
            }
            nav ul.active {
                display: flex;
            }
            nav ul li {
                margin: 0;
                text-align: center;
            }
            nav ul li a {
                display: block;
                padding: 1rem;
            }
            .mobile-menu-btn {
                display: block;
            }
            .hero h1 {
                font-size: 2.2rem;
            }
            .hero p {
                font-size: 1.1rem;
            }
            .documents-grid {
                grid-template-columns: 1fr;
            }
            .footer-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <i class="fas fa-brain"></i> Knowledge<span>Nexus</span>
            </a>
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            <nav>
                <ul id="mainNav">
                    <li><a href="#" class="active"><i class="fas fa-home"></i> Scribd Hub</a></li>
                    <li><a href="#"><i class="fas fa-crown"></i> Everand Premium</a></li>
                    <li><a href="#"><i class="fas fa-presentation"></i> SlideShare</a></li>
                    <li><a href="#" id="openUploadModal"><i class="fas fa-cloud-upload-alt"></i> Upload</a></li>
                    <li><a href="#"><i class="fas fa-user"></i> Profile</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section with Search -->
    <section class="hero">
        <div class="container">
            <h1>Share & Discover Knowledge</h1>
            <p>Access millions of documents, presentations, and research papers across all fields of study and professional practice. From University lectures to specialized Legal briefs.</p>
            <div class="search-bar">
                <input type="text" id="searchInput" placeholder="Search for documents, topics, or authors...">
                <button id="searchButton"><i class="fas fa-search"></i> Search</button>
            </div>
        </div>
    </section>

    <!-- Main Content Area -->
    <div class="container main-content">
        <!-- Sidebar with Categories -->
        <aside class="sidebar">
            <h3><i class="fas fa-layer-group"></i> Categories</h3>
            <ul class="category-list" id="categoryList">
                <!-- Categories will be dynamically populated by JavaScript -->
            </ul>
            <!-- Ad Placeholder 1 (Sidebar) -->
            <div class="ad-placeholder" style="margin-top: 2rem;">
                <i class="fas fa-ad"></i>
                <p>Advertisement Space<br>(Google AdSense Sidebar)</p>
                <!-- In production, insert Google AdSense code here -->
                <!-- <ins class="adsbygoogle" ...></ins> -->
            </div>
        </aside>

        <!-- Primary Content Area -->
        <main class="content-area">
            <!-- Ad Placeholder 2 (Top of content) -->
            <div class="ad-placeholder">
                <i class="fas fa-ad"></i>
                <p>Advertisement Space<br>(Google AdSense Leaderboard)</p>
            </div>

            <!-- Document Listing Section -->
            <div class="section-title">
                <h2><i class="fas fa-file-alt"></i> Recent Documents</h2>
                <div>
                    <button class="btn" id="openUploadModal2"><i class="fas fa-upload"></i> Upload Document</button>
                </div>
            </div>
            <div class="documents-grid" id="documentsGrid">
                <!-- Document cards will be dynamically populated by JavaScript -->
            </div>
        </main>
    </div>

    <!-- Upload Document Modal -->
    <div class="modal-overlay" id="uploadModal">
        <div class="upload-modal">
            <h3><i class="fas fa-cloud-upload-alt"></i> Upload a New Document</h3>
            <form id="documentUploadForm">
                <div class="form-group">
                    <label for="docTitle">Document Title *</label>
                    <input type="text" id="docTitle" placeholder="e.g., Introduction to Constitutional Law" required>
                </div>
                <div class="form-group">
                    <label for="docDescription">Description</label>
                    <textarea id="docDescription" rows="3" placeholder="Brief description of the document content..."></textarea>
                </div>
                <div class="form-group">
                    <label for="docCategory">Primary Category *</label>
                    <select id="docCategory" required>
                        <option value="">Select a category</option>
                        <option value="university">University</option>
                        <option value="school">School</option>
                        <option value="college">College</option>
                        <option value="law">Law</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="docSubCategory">Sub-Category / Field</label>
                    <select id="docSubCategory">
                        <option value="">Select a sub-category (if applicable)</option>
                        <!-- Sub-categories will be populated dynamically based on primary category -->
                    </select>
                </div>
                <div class="form-group">
                    <label for="docTags">Tags (comma separated)</label>
                    <input type="text" id="docTags" placeholder="e.g., contract, business, agreement">
                </div>
                <div class="form-group">
                    <label>Upload File *</label>
                    <div class="file-upload-area" id="fileUploadArea">
                        <i class="fas fa-file-pdf"></i>
                        <p><strong>Click to browse</strong> or drag and drop your file here</p>
                        <p>Supported formats: PDF, DOC, DOCX, PPT (Max 100MB)</p>
                        <input type="file" id="fileInput" accept=".pdf,.doc,.docx,.ppt,.pptx" hidden>
                        <p id="fileName" style="margin-top: 10px; color: #4361ee; font-weight: bold;"></p>
                    </div>
                </div>
                <div class="modal-actions">
                    <button type="button" class="btn btn-secondary" id="cancelUpload">Cancel</button>
                    <button type="submit" class="btn">Upload Document</button>
                </div>
            </form>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h4>Knowledge Nexus</h4>
                    <p>Your unified platform for learning, sharing, and discovery. Access documents, premium books, and presentations in one ecosystem.</p>
                </div>
                <div class="footer-column">
                    <h4>Services</h4>
                    <ul class="footer-links">
                        <li><a href="#">Scribd Document Hub</a></li>
                        <li><a href="#">Everand Premium Subscription</a></li>
                        <li><a href="#">SlideShare Presentations</a></li>
                        <li><a href="#">Ask AI Features</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h4>Legal</h4>
                    <ul class="footer-links">
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Cookie Policy</a></li>
                        <li><a href="#">Copyright Guidelines</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h4>Connect</h4>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fab fa-twitter"></i> Twitter</a></li>
                        <li><a href="#"><i class="fab fa-facebook"></i> Facebook</a></li>
                        <li><a href="#"><i class="fab fa-linkedin"></i> LinkedIn</a></li>
                        <li><a href="#"><i class="fas fa-envelope"></i> Contact Us</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Knowledge Nexus, Inc. All rights reserved. | This site is optimized for SEO and uses Google AdSense for monetization.</p>
                <p style="font-size: 0.8rem; margin-top: 5px;">Simulated prototype for demonstration purposes.</p>
            </div>
        </div>
    </footer>

    <script>
        // ===== DATA MODELS & CONFIGURATION =====
        // In a real application, this data would come from a backend API
        const platformData = {
            categories: [
                {
                    id: 'university',
                    name: 'University',
                    icon: 'fas fa-university',
                    subcategories: ['Engineering', 'Medicine', 'Arts & Humanities', 'Natural Sciences', 'Business Studies', 'Computer Science']
                },
                {
                    id: 'school',
                    name: 'School',
                    icon: 'fas fa-school',
                    subcategories: ['Mathematics', 'Science', 'Languages', 'Social Studies', 'Arts', 'Physical Education']
                },
                {
                    id: 'college',
                    name: 'College',
                    icon: 'fas fa-graduation-cap',
                    subcategories: ['Associate Degrees', 'Vocational Training', 'Continuing Education', 'Certification Programs']
                },
                {
                    id: 'law',
                    name: 'Law',
                    icon: 'fas fa-gavel',
                    subcategories: [
                        'Admiralty / Maritime Law', 'Animal Law', 'Business / Corporate Law', 
                        'Civil Rights Law', 'Constitutional Law', 'Criminal Law', 
                        'Education Law', 'Employment and Labor Law', 'Environmental Law',
                        'Family and Juvenile Law', 'First Amendment Law', 'Health Law',
                        'Immigration Law', 'Intellectual Property Law', 'International Law',
                        'Municipal Law', 'Real Estate Law', 'Securities Law',
                        'Sports and Entertainment Law', 'Tax Law'
                    ]
                }
            ],
            documents: [
                {
                    id: 1,
                    title: 'Introduction to Constitutional Law',
                    description: 'A comprehensive overview of constitutional principles and landmark cases.',
                    category: 'law',
                    subcategory: 'Constitutional Law',
                    tags: ['constitution', 'government', 'rights'],
                    uploadDate: '2023-10-15',
                    pages: 45,
                    icon: 'fas fa-file-pdf',
                    iconColor: '#e63946'
                },
                {
                    id: 2,
                    title: 'Corporate Contract Templates',
                    description: 'Collection of standard business contract templates for various purposes.',
                    category: 'law',
                    subcategory: 'Business / Corporate Law',
                    tags: ['contracts', 'business', 'templates'],
                    uploadDate: '2023-10-10',
                    pages: 120,
                    icon: 'fas fa-file-word',
                    iconColor: '#2a6fdb'
                },
                {
                    id: 3,
                    title: 'Environmental Regulations 2023',
                    description: 'Updated guide to current environmental protection laws and compliance.',
                    category: 'law',
                    subcategory: 'Environmental Law',
                    tags: ['environment', 'regulations', 'compliance'],
                    uploadDate: '2023-10-05',
                    pages: 89,
                    icon: 'fas fa-file-pdf',
                    iconColor: '#e63946'
                },
                {
                    id: 4,
                    title: 'Advanced Calculus Lecture Notes',
                    description: 'University-level calculus notes covering differential equations and integrals.',
                    category: 'university',
                    subcategory: 'Mathematics',
                    tags: ['calculus', 'mathematics', 'lecture'],
                    uploadDate: '2023-09-28',
                    pages: 67,
                    icon: 'fas fa-file-alt',
                    iconColor: '#4caf50'
                },
                {
                    id: 5,
                    title: 'Machine Learning Fundamentals',
                    description: 'Introductory presentation on ML algorithms and applications.',
                    category: 'university',
                    subcategory: 'Computer Science',
                    tags: ['AI', 'machine learning', 'algorithms'],
                    uploadDate: '2023-09-20',
                    pages: 32,
                    icon: 'fas fa-file-powerpoint',
                    iconColor: '#ff9800'
                },
                {
                    id: 6,
                    title: 'High School Biology: Genetics',
                    description: 'Complete chapter on genetics for high school biology students.',
                    category: 'school',
                    subcategory: 'Science',
                    tags: ['biology', 'genetics', 'DNA'],
                    uploadDate: '2023-09-15',
                    pages: 28,
                    icon: 'fas fa-file-pdf',
                    iconColor: '#e63946'
                }
            ]
        };

        // ===== DOM ELEMENTS =====
        const categoryListEl = document.getElementById('categoryList');
        const documentsGridEl = document.getElementById('documentsGrid');
        const uploadModal = document.getElementById('uploadModal');
        const openUploadModalBtns = document.querySelectorAll('#openUploadModal, #openUploadModal2');
        const cancelUploadBtn = document.getElementById('cancelUpload');
        const fileUploadArea = document.getElementById('fileUploadArea');
        const fileInput = document.getElementById('fileInput');
        const fileNameEl = document.getElementById('fileName');
        const docCategorySelect = document.getElementById('docCategory');
        const docSubCategorySelect = document.getElementById('docSubCategory');
        const uploadForm = document.getElementById('documentUploadForm');
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');
        const searchInput = document.getElementById('searchInput');
        const searchButton = document.getElementById('searchButton');

        // ===== INITIALIZATION =====
        document.addEventListener('DOMContentLoaded', function() {
            renderCategories();
            renderDocuments(platformData.documents);
            initEventListeners();
        });

        // ===== RENDER FUNCTIONS =====
        function renderCategories() {
            categoryListEl.innerHTML = '';
            platformData.categories.forEach(cat => {
                const li = document.createElement('li');
                li.innerHTML = `
                    <a href="#" data-category="${cat.id}">
                        <i class="${cat.icon}"></i> ${cat.name}
                    </a>
                    <ul class="subcategory-list" id="subcat-${cat.id}"></ul>
                `;
                categoryListEl.appendChild(li);
                
                // Add subcategories
                const subcatList = document.getElementById(`subcat-${cat.id}`);
                cat.subcategories.forEach(subcat => {
                    const subLi = document.createElement('li');
                    subLi.innerHTML = `<a href="#" data-category="${cat.id}" data-subcategory="${subcat}">${subcat}</a>`;
                    subcatList.appendChild(subLi);
                });
                
                // Add click event to category
                const catLink = li.querySelector('a');
                catLink.addEventListener('click', function(e) {
                    e.preventDefault();
                    const categoryId = this.getAttribute('data-category');
                    
                    // Toggle active class on category
                    document.querySelectorAll('.category-list li').forEach(item => {
                        item.classList.remove('active');
                    });
                    li.classList.add('active');
                    
                    // Filter documents by category
                    filterDocumentsByCategory(categoryId);
                });
                
                // Add click events to subcategories
                li.querySelectorAll('.subcategory-list a').forEach(subLink => {
                    subLink.addEventListener('click', function(e) {
                        e.preventDefault();
                        e.stopPropagation();
                        const categoryId = this.getAttribute('data-category');
                        const subcategory = this.getAttribute('data-subcategory');
                        
                        // Set parent category as active
                        document.querySelectorAll('.category-list li').forEach(item => {
                            item.classList.remove('active');
                        });
                        li.classList.add('active');
                        
                        // Filter documents by category and subcategory
                        filterDocumentsBySubcategory(categoryId, subcategory);
                    });
                });
            });
        }

        function renderDocuments(docs) {
            documentsGridEl.innerHTML = '';
            
            if (docs.length === 0) {
                documentsGridEl.innerHTML = `
                    <div style="grid-column: 1 / -1; text-align: center; padding: 3rem; color: #6c757d;">
                        <i class="fas fa-file-search" style="font-size: 3rem; margin-bottom: 1rem;"></i>
                        <h3>No documents found</h3>
                        <p>Try a different category or search term.</p>
                    </div>
                `;
                return;
            }
            
            docs.forEach(doc => {
                const card = document.createElement('div');
                card.className = 'document-card';
                card.innerHTML = `
                    <div class="doc-thumbnail" style="background-color: ${doc.iconColor}20;">
                        <i class="${doc.icon}" style="color: ${doc.iconColor};"></i>
                    </div>
                    <div class="doc-info">
                        <h4>${doc.title}</h4>
                        <p>${doc.description}</p>
                        <div class="doc-meta">
                            <span><i class="fas fa-tag"></i> ${doc.subcategory}</span>
                            <span><i class="far fa-calendar"></i> ${doc.uploadDate}</span>
                        </div>
                        <div class="doc-meta" style="margin-top: 0.5rem;">
                            <span><i class="fas fa-file"></i> ${doc.pages} pages</span>
                            <button class="btn" style="padding: 5px 12px; font-size: 0.8rem;" onclick="viewDocument(${doc.id})">View</button>
                        </div>
                    </div>
                `;
                documentsGridEl.appendChild(card);
            });
        }

        // ===== DOCUMENT FILTERING =====
        function filterDocumentsByCategory(categoryId) {
            const filtered = platformData.documents.filter(doc => doc.category === categoryId);
            renderDocuments(filtered);
            updateSectionTitle(`${getCategoryName(categoryId)} Documents`);
        }

        function filterDocumentsBySubcategory(categoryId, subcategory) {
            const filtered = platformData.documents.filter(doc => 
                doc.category === categoryId && doc.subcategory === subcategory
            );
            renderDocuments(filtered);
            updateSectionTitle(`${subcategory} Documents`);
        }

        function searchDocuments(query) {
            const lowerQuery = query.toLowerCase().trim();
            if (!lowerQuery) {
                renderDocuments(platformData.documents);
                updateSectionTitle('Recent Documents');
                return;
            }
            
            const filtered = platformData.documents.filter(doc => 
                doc.title.toLowerCase().includes(lowerQuery) ||
                doc.description.toLowerCase().includes(lowerQuery) ||
                doc.tags.some(tag => tag.toLowerCase().includes(lowerQuery)) ||
                doc.subcategory.toLowerCase().includes(lowerQuery)
            );
            
            renderDocuments(filtered);
            updateSectionTitle(`Search Results for "${query}"`);
        }

        function getCategoryName(categoryId) {
            const cat = platformData.categories.find(c => c.id === categoryId);
            return cat ? cat.name : categoryId;
        }

        function updateSectionTitle(title) {
            const titleEl = document.querySelector('.section-title h2');
            if (titleEl) {
                titleEl.innerHTML = `<i class="fas fa-file-alt"></i> ${title}`;
            }
        }

        // ===== MODAL & UPLOAD FUNCTIONALITY =====
        function initEventListeners() {
            // Open upload modal
            openUploadModalBtns.forEach(btn => {
                btn.addEventListener('click', () => {
                    uploadModal.classList.add('active');
                });
            });
            
            // Close upload modal
            cancelUploadBtn.addEventListener('click', () => {
                uploadModal.classList.remove('active');
                resetUploadForm();
            });
            
            // Close modal when clicking outside
            uploadModal.addEventListener('click', (e) => {
                if (e.target === uploadModal) {
                    uploadModal.classList.remove('active');
                    resetUploadForm();
                }
            });
            
            // File upload area interaction
            fileUploadArea.addEventListener('click', () => {
                fileInput.click();
            });
            
            fileInput.addEventListener('change', (e) => {
                if (fileInput.files.length > 0) {
                    fileNameEl.textContent = `Selected: ${fileInput.files[0].name}`;
                    fileUploadArea.style.borderColor = '#4361ee';
                    fileUploadArea.style.backgroundColor = '#eef2
                }
            });
            
            // Drag and drop for file upload
            fileUploadArea.addEventListener('dragover', (e) => {
                e.preventDefault();
                fileUploadArea.classList.add('dragover');
            });
            
            fileUploadArea.addEventListener('dragleave', () => {
                fileUploadArea.classList.remove('dragover');
            });
            
            fileUploadArea.addEventListener('drop', (e) => {
                e.preventDefault();
                fileUploadArea.classList.remove('dragover');
                
                if (e.dataTransfer.files.length > 0) {
                    fileInput.files = e.dataTransfer.files;
                    fileNameEl.textContent = `Selected: ${e.dataTransfer.files[0].name}`;
                    fileUploadArea.style.borderColor = '#4361ee';
                    fileUploadArea.style.backgroundColor = '#eef2ff';
                }
            });
            
            // Update subcategories when category changes
            docCategorySelect.addEventListener('change', function() {
                const categoryId = this.value;
                const category = platformData.categories.find(c => c.id === categoryId);
                
                // Clear and disable subcategory select
                docSubCategorySelect.innerHTML = '<option value="">Select a sub-category (if applicable)</option>';
                
                if (category) {
                    // Enable and populate subcategories
                    category.subcategories.forEach(subcat => {
                        const option = document.createElement('option');
                        option.value = subcat;
                        option.textContent = subcat;
                        docSubCategorySelect.appendChild(option);
                    });
                    docSubCategorySelect.disabled = false;
                } else {
                    docSubCategorySelect.disabled = true;
                }
            });
            
            // Handle form submission
            uploadForm.addEventListener('submit', (e) => {
                e.preventDefault();
                
                // Get form values
                const title = document.getElementById('docTitle').value;
                const description = document.getElementById('docDescription').value;
                const category = docCategorySelect.value;
                const subcategory = docSubCategorySelect.value;
                const tags = document.getElementById('docTags').value.split(',').map(tag => tag.trim()).filter(tag => tag);
                const file = fileInput.files[0];
                
                // Simple validation
                if (!file) {
                    alert('Please select a file to upload.');
                    return;
                }
                
                // Simulate upload success
                console.log('Uploading document:', { title, description, category, subcategory, tags, fileName: file.name });
                
                // Show success message
                alert(`Document "${title}" uploaded successfully! (This is a simulation - in production, file would be sent to backend)`);
                
                // Close modal and reset form
                uploadModal.classList.remove('active');
                resetUploadForm();
                
                // In a real app, you would refresh the document list from the backend
                // For simulation, add the new document to the local list
                const newDoc = {
                    id: platformData.documents.length + 1,
                    title,
                    description,
                    category,
                    subcategory: subcategory || 'General',
                    tags,
                    uploadDate: new Date().toISOString().split('T')[0],
                    pages: Math.floor(Math.random() * 100) + 10,
                    icon: 'fas fa-file-pdf',
                    iconColor: '#e63946'
                };
                
                platformData.documents.unshift(newDoc);
                filterDocumentsByCategory(category);
            });
            
            // Mobile menu toggle
            mobileMenuBtn.addEventListener('click', () => {
                mainNav.classList.toggle('active');
                mobileMenuBtn.innerHTML = mainNav.classList.contains('active') 
                    ? '<i class="fas fa-times"></i>' 
                    : '<i class="fas fa-bars"></i>';
            });
            
            // Search functionality
            searchButton.addEventListener('click', () => {
                searchDocuments(searchInput.value);
            });
            
            searchInput.addEventListener('keyup', (e) => {
                if (e.key === 'Enter') {
                    searchDocuments(searchInput.value);
                }
            });
        }

        function resetUploadForm() {
            uploadForm.reset();
            fileNameEl.textContent = '';
            fileUploadArea.style.borderColor = '';
            fileUploadArea.style.backgroundColor = '';
            docSubCategorySelect.innerHTML = '<option value="">Select a sub-category (if applicable)</option>';
            docSubCategorySelect.disabled = true;
        }

        // ===== DOCUMENT VIEW SIMULATION =====
        function viewDocument(docId) {
            // In production, this would redirect to a document viewer page
            // For simulation, show an ad modal before "viewing" the document
            
            // Create ad modal
            const adModal = document.createElement('div');
            adModal.className = 'modal-overlay active';
            adModal.innerHTML = `
                <div class="upload-modal" style="max-width: 500px;">
                    <h3><i class="fas fa-ad"></i> Advertisement</h3>
                    <p style="text-align: center; margin: 2rem 0;">
                        This content is supported by advertisements. Please watch a short ad to continue.
                    </p>
                    <div class="ad-placeholder" style="margin: 1.5rem 0; padding: 3rem;">
                        <i class="fas fa-ad" style="font-size: 3rem;"></i>
                        <p>Google AdSense Video Ad<br>(Simulated - 5 seconds)</p>
                        <div id="countdown" style="font-size: 2rem; font-weight: bold; color: #4361ee; margin-top: 1rem;">5</div>
                    </div>
                    <p style="text-align: center; color: #6c757d; font-size: 0.9rem;">
                        Thank you for supporting free access to knowledge.
                    </p>
                    <div class="modal-actions">
                        <button id="skipAdBtn" class="btn btn-secondary">Skip Ad (for Premium)</button>
                        <button id="closeAdBtn" class="btn" disabled>Continue in <span id="continueCount">5</span>s</button>
                    </div>
                </div>
            `;
            
            document.body.appendChild(adModal);
            
            // Countdown logic
            let countdown = 5;
            const countdownEl = adModal.querySelector('#countdown');
            const continueCountEl = adModal.querySelector('#continueCount');
            const closeAdBtn = adModal.querySelector('#closeAdBtn');
            const skipAdBtn = adModal.querySelector('#skipAdBtn');
            
            const countdownInterval = setInterval(() => {
                countdown--;
                countdownEl.textContent = countdown;
                continueCountEl.textContent = countdown;
                
                if (countdown <= 0) {
                    clearInterval(countdownInterval);
                    closeAdBtn.textContent = 'Continue to Document';
                    closeAdBtn.disabled = false;
                }
            }, 1000);
            
            // Close ad and proceed to document
            closeAdBtn.addEventListener('click', () => {
                document.body.removeChild(adModal);
                // In production, redirect to actual document viewer
                alert(`Now viewing document ID: ${docId}\n\nIn production, this would open the document viewer with the actual content.`);
            });
            
            // Skip ad (premium feature simulation)
            skipAdBtn.addEventListener('click', () => {
                clearInterval(countdownInterval);
                document.body.removeChild(adModal);
                alert('Ad skipped (Premium feature). Redirecting to document...\n\nIn production, this would verify user subscription status.');
                alert(`Now viewing document ID: ${docId}\n\nIn production, this would open the document viewer with the actual content.`);
            });
            
            // Close modal when clicking outside (disabled for ad)
            adModal.addEventListener('click', (e) => {
                if (e.target === adModal) {
                    // Don't allow closing by clicking outside during ad
                    // In production, you might want to handle this differently
                }
            });
        }
    </script>
</body>
</html>
