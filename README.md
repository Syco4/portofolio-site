export default function PortfolioSite() {
  return (
    <main className="bg-white text-gray-800 font-sans">
      {/* Header */}
      <header className="bg-gray-100 py-6 shadow-md">
        <div className="max-w-6xl mx-auto px-4 flex justify-between items-center">
          <h1 className="text-2xl font-bold">استوديو الإبداع</h1>
          <nav className="space-x-4 rtl:space-x-reverse">
            <a href="#home" className="text-gray-700 hover:text-black">الرئيسية</a>
            <a href="#portfolio" className="text-gray-700 hover:text-black">أعمالي</a>
            <a href="#about" className="text-gray-700 hover:text-black">من أنا</a>
            <a href="#contact" className="text-gray-700 hover:text-black">تواصل</a>
          </nav>
        </div>
      </header>

      {/* Hero Section */}
      <section id="home" className="py-20 bg-gradient-to-r from-gray-200 to-gray-100">
        <div className="max-w-6xl mx-auto px-4 text-center">
          <h2 className="text-4xl font-extrabold mb-4">مرحباً بك في عالمي الإبداعي</h2>
          <p className="text-lg text-gray-600 mb-6">
            أصمم لك هوية بصرية تلفت الأنظار، وأعمالاً تليق بطموحاتك.
          </p>
          <a href="#portfolio" className="bg-black text-white py-2 px-6 rounded-lg hover:bg-gray-800 transition">
            تصفح أعمالي
          </a>
        </div>
      </section>

      {/* Portfolio Section */}
      <section id="portfolio" className="py-16">
        <div className="max-w-6xl mx-auto px-4">
          <h3 className="text-3xl font-bold mb-10 text-center">أعمالي السابقة</h3>
          <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
            {/* Example Project Cards */}
            <div className="border rounded-lg overflow-hidden shadow-sm">
              <img src="/project1.jpg" alt="مشروع 1" className="w-full h-48 object-cover" />
              <div className="p-4">
                <h4 className="font-semibold text-lg mb-2">تصميم شعار احترافي</h4>
                <p className="text-gray-600">شعار فريد لعلامة تجارية حديثة.</p>
              </div>
            </div>
            <div className="border rounded-lg overflow-hidden shadow-sm">
              <img src="/project2.jpg" alt="مشروع 2" className="w-full h-48 object-cover" />
              <div className="p-4">
                <h4 className="font-semibold text-lg mb-2">هوية بصرية كاملة</h4>
                <p className="text-gray-600">هوية متكاملة تشمل الشعار والألوان والخطوط.</p>
              </div>
            </div>
            <div className="border rounded-lg overflow-hidden shadow-sm">
              <img src="/project3.jpg" alt="مشروع 3" className="w-full h-48 object-cover" />
              <div className="p-4">
                <h4 className="font-semibold text-lg mb-2">تصميم سوشيال ميديا</h4>
                <p className="text-gray-600">قوالب جذابة لمنصات التواصل الاجتماعي.</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* About Section */}
      <section id="about" className="py-16 bg-gray-100">
        <div className="max-w-4xl mx-auto px-4 text-center">
          <h3 className="text-3xl font-bold mb-6">من أنا</h3>
          <p className="text-gray-700 text-lg">
            أنا مصمم جرافيك حر من الجزائر، أقدم خدمات التصميم بأسلوب عصري واحترافي. أعمل بشغف على تحويل الأفكار إلى تصاميم تُلهم وتُميز. لدي خبرة واسعة في تصميم الشعارات، الهوية البصرية، والمحتوى الرقمي.
          </p>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-16">
        <div className="max-w-4xl mx-auto px-4 text-center">
          <h3 className="text-3xl font-bold mb-6">تواصل معي</h3>
          <p className="text-gray-700 mb-4">هل لديك مشروع أو فكرة؟ يسعدني العمل معك!</p>
          <form className="space-y-4 max-w-md mx-auto">
            <input type="text" placeholder="الاسم" className="w-full p-3 border rounded-lg" />
            <input type="email" placeholder="البريد الإلكتروني" className="w-full p-3 border rounded-lg" />
            <textarea placeholder="رسالتك" className="w-full p-3 border rounded-lg h-32"></textarea>
            <button type="submit" className="bg-black text-white py-2 px-6 rounded-lg hover:bg-gray-800 transition">
              إرسال
            </button>
          </form>
        </div>
      </section>

      {/* Footer */}
      <footer className="py-6 bg-gray-100 text-center text-gray-600">
        &copy; {new Date().getFullYear()} استوديو الإبداع - جميع الحقوق محفوظة.
      </footer>
    </main>
  );
}

