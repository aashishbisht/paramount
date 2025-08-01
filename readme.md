# Shopify Store URL
paramountshpfy.myshopify.com

# Shopify Commands
shopify login paramountshpfy.myshopify.com


# Final CSS Architecture for Paramount Theme

## CSS Files Structure:

assets/
├── theme.css (base styles, utilities, typography - ALWAYS LOADED)
├── theme-header.css (navigation, header layouts - ALWAYS LOADED)
├── theme-footer.css (footer styles, social links - ALWAYS LOADED)
├── sections-core.css (hero, features, testimonials, about)
├── sections-product.css (product grids, product cards, reviews)
├── sections-collection.css (collection grids, filters, sorting)
├── sections-blog.css (blog layouts, article cards, author info)
├── sections-content.css (FAQ, contact, text-heavy pages)
├── sections-forms.css (contact forms, newsletter, search)
├── sections-cart.css (cart drawer, cart page, mini-cart)
├── sections-checkout.css (checkout process, payment forms)
└── sections-specialty.css (advanced animations, complex layouts)

## Loading Strategy by Performance Zone:

### **Critical (Always Load):**
- `theme.css`
- `theme-header.css`
- `theme-footer.css`

### **Page-Type Specific:**
- `sections-product.css` → Product/Collection pages
- `sections-collection.css` → Collection pages only
- `sections-blog.css` → Blog/Article pages
- `sections-content.css` → Static pages (About, Contact, etc.)

### **Interaction-Based (Load on Demand):**
- `sections-forms.css` → Pages with forms
- `sections-cart.css` → When cart functionality present
- `sections-checkout.css` → Checkout flow only

### **Section-Based (Dynamic Loading):**
- `sections-core.css` → When hero/features/testimonials used
- `sections-specialty.css` → When advanced sections used

## File Contents Overview:

### **theme.css**
- CSS reset & normalize
- Typography system
- Color variables
- Grid & flexbox utilities
- Button base styles
- Form base styles
- Responsive utilities

### **theme-header.css**
- Header layouts
- Navigation styles
- Mobile menu
- Search functionality
- Logo positioning

### **theme-footer.css**
- Footer layouts
- Social media links
- Newsletter signup
- Footer navigation

### **sections-core.css**
- Hero sections
- Feature sections
- Testimonial layouts
- About sections
- CTA sections

### **sections-product.css**
- Product grids
- Product cards
- Product images
- Quick view
- Product badges
- Review stars

### **sections-collection.css**
- Collection grids
- Filter sidebar
- Sort dropdown
- Pagination
- Collection headers

### **sections-blog.css**
- Blog grid layouts
- Article cards
- Author bio
- Related articles
- Blog sidebar

### **sections-content.css**
- FAQ accordions
- Text content layouts
- Image + text sections
- Timeline layouts
- Icon + text sections

### **sections-forms.css**
- Contact forms
- Newsletter forms
- Search forms
- Form validation styles
- Input styling

### **sections-cart.css**
- Cart drawer
- Cart page layout
- Mini cart popup
- Cart item styles
- Quantity selectors

### **sections-checkout.css**
- Checkout layouts
- Payment forms
- Shipping options
- Order summary
- Progress indicators

### **sections-specialty.css**
- Advanced animations
- Complex hover effects
- Parallax sections
- Video backgrounds
- Custom cursors