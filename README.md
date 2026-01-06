# 🍽️ UniHub - College Canteen Preordering System

A comprehensive web-based food preordering system designed for college canteens, enabling students and staff to browse menus, place orders, and make payments seamlessly.

## 📋 Table of Contents
- [Features](#features)
- [System Architecture](#system-architecture)
- [Canteen Types](#canteen-types)
- [Installation](#installation)
- [Usage](#usage)
- [User Roles](#user-roles)
- [File Structure](#file-structure)
- [Technologies Used](#technologies-used)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

### 🔐 Authentication System
- **Dual Role Login**: Students and Canteen Head access
- **Student Login**: VIT email format authentication (@vit.edu)
- **Canteen Head Login**: Individual canteen management access
- **Password Toggle**: Show/hide password functionality

### 🏪 Multi-Canteen Support
- **4 Different Canteens**: Each with unique menus and specialties
- **Real-time Menu Management**: Canteen heads can update availability
- **Search Functionality**: Find food items quickly across menus
- **Responsive Design**: Works on desktop and mobile devices

### 🛒 Shopping Cart System
- **Add/Remove Items**: Easy cart management
- **Quantity Control**: Adjust item quantities
- **Real-time Total**: Live price calculation
- **Persistent Cart**: Cart data maintained during session

### 💳 Payment Integration
- **QR Code Payments**: Quick payment via QR scanning
- **Order Summary**: Detailed breakdown of items and prices
- **Digital Receipts**: Downloadable payment receipts
- **Receipt History**: Stored in local storage for reference

### 📱 User Experience
- **Intuitive Navigation**: Easy-to-use interface
- **Visual Menu Display**: High-quality food images
- **Mobile Responsive**: Optimized for all screen sizes
- **Fast Loading**: Optimized performance

## 🏗️ System Architecture

```
UniHub System
├── Authentication Layer
│   ├── Student Login (@vit.edu)
│   └── Canteen Head Login
├── Main Dashboard
│   └── Canteen Selection Interface
├── Canteen Modules
│   ├── Main Canteen
│   ├── Staff Canteen
│   ├── Fruit Canteen
│   └── Kiosk Café
└── Payment System
    ├── Order Processing
    ├── QR Code Integration
    └── Receipt Generation
```

## 🍕 Canteen Types

### 1. **Main Canteen** 🍛
- **Specialties**: Indian meals, breakfast items, rice dishes
- **Categories**: Paratha, Dosa, Breakfast, Hot/Cold Beverages, Sandwiches, Starters
- **Popular Items**: Vada Pav (₹16), Samosa (₹17), Pav Bhaji (₹50)

### 2. **Staff Canteen** 👨‍🏫
- **Target**: Faculty and staff members
- **Categories**: Drinks, Lunch meals (J1), Breakfast items (Nashta)
- **Features**: Budget-friendly options, traditional Indian meals

### 3. **Fruit Canteen** 🍓
- **Specialties**: Fresh juices, shakes, healthy snacks
- **Categories**: Shakes, Juices, Sandwiches, Parathas, Fresh Foods
- **Health Focus**: Natural ingredients, fresh fruit preparations

### 4. **Kiosk Café** ☕
- **Specialties**: Premium beverages, international drinks
- **Categories**: Hot Beverages, Cold Beverages, Shakes, Mojitos, Hot Chocolate
- **Premium Options**: Specialty coffee, gourmet shakes, signature beverages

## 🚀 Installation

### Prerequisites
- Web browser (Chrome, Firefox, Safari, Edge)
- Local web server (optional, for development)

### Setup Instructions

1. **Clone/Download the Repository**
   ```bash
   git clone <repository-url>
   cd Pre-Ordering-Food-Canteen
   ```

2. **File Structure Setup**
   - Ensure all HTML files are in the root directory
   - Verify Assets folder contains all images and media files
   - Check that all image paths are correctly referenced

3. **Launch the Application**
   - Open `index.html` in your web browser
   - Or set up a local server and navigate to the project directory

4. **For Development Server (Optional)**
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

## 📖 Usage

### For Students

1. **Login Process**
   - Open the application via `index.html`
   - Select "Student" role
   - Enter VIT email ID (@vit.edu format)
   - Use the same email as password
   - Click Login

2. **Ordering Food**
   - Select desired canteen from the main dashboard
   - Browse through food categories
   - Use search bar to find specific items
   - Add items to cart with quantity selection
   - Review cart and proceed to checkout

3. **Payment Process**
   - Review order summary on payment page
   - Scan QR code for payment
   - Generate and save digital receipt

### For Canteen Heads

1. **Login Process**
   - Select "Canteen Head" role
   - Use canteen credentials (canteen1-canteen6)
   - Access respective canteen management panel

2. **Menu Management**
   - Update item availability
   - Modify prices (if applicable)
   - View order statistics

## 👥 User Roles

### 🎓 Student Role
- **Access**: All canteen menus
- **Permissions**: Browse, order, payment
- **Authentication**: VIT email format
- **Features**: Cart management, order history, receipt generation

### 👨‍💼 Canteen Head Role
- **Access**: Specific canteen management
- **Permissions**: Menu updates, availability control
- **Authentication**: Canteen-specific credentials
- **Features**: Inventory management, order tracking

## 📁 File Structure

```
00_ASEP1_WEBSITE/
├── 📄 index.html               # Authentication entry point
├── 📄 main_page.html           # Canteen selection dashboard
├── 📄 main_canteen.html        # Main canteen menu
├── 📄 staff_canteen.html       # Staff canteen menu
├── 📄 fruit_canteen.html       # Fruit canteen menu
├── 📄 koisk.html              # Kiosk café menu
├── 📄 payment_main_page.html   # Main canteen payment
├── 📄 payment_staff_page.html  # Staff canteen payment
├── 📄 payment_fruit_page.html  # Fruit canteen payment
├── 📄 payment_koisk_page.html  # Kiosk payment
├── 📄 canteen1.html           # Canteen head panel 1
├── 📄 canteen2.html           # Canteen head panel 2
├── 📄 canteen3.html           # Canteen head panel 3
├── 📄 canteen4.html           # Canteen head panel 4
└── 📁 Assets/
    ├── 📁 Main canteen/        # Main canteen images
    ├── 📁 Staff canteen/       # Staff canteen images
    ├── 📁 FC/                  # Fruit canteen images
    ├── 📁 kisok caffe/         # Kiosk café images
    └── 📁 Other/               # Common assets (logos, backgrounds)
```

## 💻 Technologies Used

### Frontend
- **HTML5**: Structure and semantic markup
- **CSS3**: Styling, animations, and responsive design
- **JavaScript (ES6+)**: Interactive functionality and DOM manipulation
- **Google Fonts**: Poppins font family for modern typography

### Features Implementation
- **Local Storage**: Cart persistence and user data
- **Responsive Design**: CSS Grid and Flexbox
- **CSS Animations**: Smooth transitions and hover effects
- **Form Validation**: Client-side authentication
- **URL Parameters**: Order data transfer between pages

### Design Elements
- **CSS Grid**: Layout management
- **Flexbox**: Component alignment
- **Media Queries**: Mobile responsiveness
- **CSS Variables**: Consistent theming
- **Transform Animations**: Interactive feedback

## 🔧 Configuration

### Login Credentials

#### Student Access
- **Format**: `<name>@vit.edu`
- **Password**: Same as username
- **Example**: `john.doe@vit.edu` / `john.doe@vit.edu`

#### Canteen Head Access
- **Canteen 1**: `canteen1` / `canteen1`
- **Canteen 2**: `canteen2` / `canteen2`
- **Canteen 3**: `canteen3` / `canteen3`
- **Canteen 4**: `canteen4` / `canteen4`

### Customization Options

1. **Menu Items**: Edit product arrays in respective HTML files
2. **Pricing**: Modify price values in JavaScript objects
3. **Images**: Replace images in Assets folders (maintain naming convention)
4. **Styling**: Update CSS variables for theme customization
5. **Payment QR**: Replace QR code images with actual payment gateway QRs

## 🤝 Contributing

We welcome contributions to improve UniHub! Here's how you can help:

### Development Setup
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Test thoroughly across different browsers
5. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
6. Push to the branch (`git push origin feature/AmazingFeature`)
7. Open a Pull Request

### Contribution Guidelines
- Follow existing code style and structure
- Test on multiple browsers and devices
- Update documentation for new features
- Ensure responsive design compatibility
- Optimize images and assets

### Areas for Improvement
- Backend integration for real-time data
- Payment gateway integration
- Order tracking system
- Admin dashboard enhancements
- Mobile app development
- Database integration
- User feedback system


## 🚀 Future Enhancements

- **Real-time Order Tracking**: Live status updates
- **Payment Gateway Integration**: Multiple payment options
- **Admin Analytics**: Sales and order analytics
- **Mobile Application**: Native iOS/Android apps
- **Notification System**: Order status notifications
- **Loyalty Program**: Student reward system
- **Inventory Management**: Real-time stock tracking
- **Multi-language Support**: Regional language options

---

**Made with ❤️ for VIT College Community**

*UniHub - Simplifying campus dining, one order at a time.*
