# Hamo-2003 Portfolio

موقع شخصي احترافي لمهندس زراعي متخصص في تطوير الأدوات والحلول الزراعية الذكية.

**[English](#english-version) | [العربية](#النسخة-العربية)**

---

## النسخة العربية

### 🌟 المميزات

- **تصميم حديث وجذاب**: واجهة مستخدم احترافية بتصميم داكن مع تدرجات لونية جميلة
- **دعم اللغتين**: النسخة العربية والإنجليزية مع دعم RTL كامل
- **نظام تبديل اللغة**: تبديل سلس بين العربية والإنجليزية على جميع الصفحات
- **أدوات متخصصة**: 
  - حاسبة وحدات العناصر من الأسمدة
  - مولد روابط واتساب احترافي
- **استجابة كاملة**: تصميم متجاوب يعمل على جميع الأجهزة
- **أداء عالي**: بناء سريع باستخدام Vite و React 19

### 🛠️ التقنيات المستخدمة

- **Frontend**: React 19 + TypeScript
- **Styling**: Tailwind CSS 4 + shadcn/ui
- **Routing**: Wouter
- **State Management**: React Context API
- **Build Tool**: Vite
- **Language Support**: Custom i18n system

### 📁 هيكل المشروع

```
hamo-2003-portfolio/
├── client/
│   ├── src/
│   │   ├── pages/           # صفحات التطبيق
│   │   │   ├── Home.tsx     # الصفحة الرئيسية
│   │   │   └── FertilizerCalculator.tsx  # حاسبة الأسمدة
│   │   ├── components/      # مكونات قابلة لإعادة الاستخدام
│   │   ├── contexts/        # React Contexts
│   │   │   └── LanguageContext.tsx  # نظام إدارة اللغة
│   │   ├── App.tsx          # المكون الرئيسي
│   │   └── main.tsx         # نقطة الدخول
│   └── public/              # الملفات الثابتة
├── package.json
└── tsconfig.json
```

### 🚀 البدء السريع

#### المتطلبات
- Node.js 18+
- npm أو pnpm

#### التثبيت والتشغيل

```bash
# استنساخ المشروع
git clone https://github.com/hamo-2003/hamo-2003-portfolio.git
cd hamo-2003-portfolio

# تثبيت الحزم
npm install
# أو
pnpm install

# تشغيل خادم التطوير
npm run dev
# أو
pnpm dev

# سيتم فتح الموقع على http://localhost:5173
```

#### البناء للإنتاج

```bash
npm run build
# أو
pnpm build

# المخرجات ستكون في مجلد dist/
```

### 🌐 نظام اللغة

يستخدم المشروع نظام Context API مخصص لإدارة اللغة:

```typescript
import { useLanguage } from '@/contexts/LanguageContext';

export default function MyComponent() {
  const { language, setLanguage, t } = useLanguage();
  
  return (
    <div>
      <p>{t('nav.about')}</p>
      <button onClick={() => setLanguage('ar')}>العربية</button>
      <button onClick={() => setLanguage('en')}>English</button>
    </div>
  );
}
```

### 📱 الأدوات المتضمنة

#### 1. حاسبة وحدات العناصر من الأسمدة
- حساب كمية السماد المطلوبة بناءً على عدد الوحدات
- دعم 18 نوع سماد مختلف
- تصدير النتائج (CSV, Excel)
- طباعة النتائج
- واجهة بسيطة وسهلة الاستخدام

#### 2. مولد روابط واتساب
- إنشاء روابط واتساب احترافية
- دعم الملفات (Excel, Word)
- واجهة سهلة الاستخدام

### 🎨 التخصيص

#### تغيير الألوان
عدّل ملف `client/src/index.css` لتغيير نظام الألوان:

```css
@theme {
  --color-primary: oklch(0.6 0.2 240);
  --color-secondary: oklch(0.7 0.15 200);
}
```

#### إضافة ترجمات جديدة
أضف مفاتيح جديدة في `client/src/contexts/LanguageContext.tsx`:

```typescript
const translations = {
  ar: {
    "your.key": "النص العربي",
  },
  en: {
    "your.key": "English text",
  }
};
```

### 📊 الأداء

- **Lighthouse Score**: 90+
- **Core Web Vitals**: جميعها خضراء
- **Build Size**: ~150KB (gzipped)

### 🔐 الأمان

- لا توجد بيانات حساسة في الكود
- جميع البيانات تُعالج محلياً في المتصفح
- لا توجد طلبات API خارجية

### 📝 الترخيص

هذا المشروع مرخص تحت رخصة MIT.

### 👤 المؤلف

**محمد صبحي** - مهندس زراعي ومطور ويب

- GitHub: [@hamo-2003](https://github.com/hamo-2003)
- البريد الإلكتروني: [بريدك الإلكتروني]
- LinkedIn: [ملفك على LinkedIn]

### 🤝 المساهمة

نرحب بالمساهمات! يرجى:

1. Fork المشروع
2. إنشاء فرع للميزة الجديدة (`git checkout -b feature/AmazingFeature`)
3. Commit التغييرات (`git commit -m 'Add some AmazingFeature'`)
4. Push إلى الفرع (`git push origin feature/AmazingFeature`)
5. فتح Pull Request

### 📞 التواصل

- **البريد الإلكتروني**: [بريدك الإلكتروني]
- **GitHub Issues**: للإبلاغ عن المشاكل والاقتراحات

---

## English Version

### 🌟 Features

- **Modern Design**: Professional UI with dark theme and beautiful gradients
- **Bilingual Support**: Full Arabic and English support with RTL support
- **Language Switching**: Seamless language switching across all pages
- **Specialized Tools**:
  - Fertilizer Nutrient Unit Calculator
  - Professional WhatsApp Link Generator
- **Fully Responsive**: Works perfectly on all devices
- **High Performance**: Fast build using Vite and React 19

### 🛠️ Technologies Used

- **Frontend**: React 19 + TypeScript
- **Styling**: Tailwind CSS 4 + shadcn/ui
- **Routing**: Wouter
- **State Management**: React Context API
- **Build Tool**: Vite
- **Language Support**: Custom i18n system

### 📁 Project Structure

```
hamo-2003-portfolio/
├── client/
│   ├── src/
│   │   ├── pages/           # Application pages
│   │   │   ├── Home.tsx     # Home page
│   │   │   └── FertilizerCalculator.tsx  # Fertilizer calculator
│   │   ├── components/      # Reusable components
│   │   ├── contexts/        # React Contexts
│   │   │   └── LanguageContext.tsx  # Language management system
│   │   ├── App.tsx          # Main component
│   │   └── main.tsx         # Entry point
│   └── public/              # Static files
├── package.json
└── tsconfig.json
```

### 🚀 Quick Start

#### Requirements
- Node.js 18+
- npm or pnpm

#### Installation & Running

```bash
# Clone the project
git clone https://github.com/hamo-2003/hamo-2003-portfolio.git
cd hamo-2003-portfolio

# Install dependencies
npm install
# or
pnpm install

# Run development server
npm run dev
# or
pnpm dev

# Open http://localhost:5173
```

#### Build for Production

```bash
npm run build
# or
pnpm build

# Output will be in dist/ folder
```

### 🌐 Language System

The project uses a custom Context API system for language management:

```typescript
import { useLanguage } from '@/contexts/LanguageContext';

export default function MyComponent() {
  const { language, setLanguage, t } = useLanguage();
  
  return (
    <div>
      <p>{t('nav.about')}</p>
      <button onClick={() => setLanguage('ar')}>العربية</button>
      <button onClick={() => setLanguage('en')}>English</button>
    </div>
  );
}
```

### 📱 Included Tools

#### 1. Fertilizer Nutrient Unit Calculator
- Calculate fertilizer quantity based on required units
- Support for 18 different fertilizer types
- Export results (CSV, Excel)
- Print results
- Simple and user-friendly interface

#### 2. WhatsApp Link Generator
- Create professional WhatsApp links
- File support (Excel, Word)
- Easy-to-use interface

### 🎨 Customization

#### Change Colors
Edit `client/src/index.css` to change the color scheme:

```css
@theme {
  --color-primary: oklch(0.6 0.2 240);
  --color-secondary: oklch(0.7 0.15 200);
}
```

#### Add New Translations
Add new keys in `client/src/contexts/LanguageContext.tsx`:

```typescript
const translations = {
  ar: {
    "your.key": "النص العربي",
  },
  en: {
    "your.key": "English text",
  }
};
```

### 📊 Performance

- **Lighthouse Score**: 90+
- **Core Web Vitals**: All green
- **Build Size**: ~150KB (gzipped)

### 🔐 Security

- No sensitive data in code
- All data processed locally in browser
- No external API calls

### 📝 License

This project is licensed under the MIT License.

### 👤 Author

**Mohamed Sobhy** - Agricultural Engineer & Web Developer

- GitHub: [@hamo-2003](https://github.com/hamo-2003)
- Email: [your-email]
- LinkedIn: [your-linkedin]

### 🤝 Contributing

We welcome contributions! Please:

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### 📞 Contact

- **Email**: [your-email]
- **GitHub Issues**: For bug reports and suggestions

---

**Made with ❤️ by Mohamed Sobhy**
