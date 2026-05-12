# For-Mummum-export default function BirthdayWebsite() {
  return (
    <div className="w-full min-h-screen bg-[#F9A7B0] overflow-hidden flex items-center justify-center relative font-sans">
      {/* BACKGROUND BLUR */}
      <div className="absolute inset-0 backdrop-blur-sm"></div>

      {/* ENVELOPE CONTAINER */}
      <div className="relative w-[350px] h-[350px] flex items-center justify-center">

        {/* TOP ENVELOPE */}
        <div className="absolute rotate-[-20deg] top-10 z-10 transition-all duration-700 hover:scale-105">
          <div className="relative w-[220px] h-[140px] bg-[#FDE4D0] border-2 border-[#5C4033] rounded-md overflow-hidden">

            {/* FLAP */}
            <div className="absolute top-0 left-0 w-full h-full origin-top bg-[#FDE4D0] border-b-2 border-[#5C4033] clip-path-triangle z-20"></div>

            {/* HEART */}
            <div className="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 z-30 animate-pulse">
              <div className="w-10 h-10 bg-pink-500 rotate-45 relative rounded-sm">
                <div className="absolute w-10 h-10 bg-pink-500 rounded-full -top-5 left-0"></div>
                <div className="absolute w-10 h-10 bg-pink-500 rounded-full left-5 top-0"></div>
              </div>
            </div>
          </div>
        </div>

        {/* BOTTOM ENVELOPE */}
        <div className="absolute rotate-[10deg] bottom-10 z-0 transition-all duration-700 hover:scale-105">
          <div className="relative w-[220px] h-[140px] bg-[#FDE4D0] border-2 border-[#5C4033] rounded-md overflow-hidden">
            <div className="absolute top-0 left-0 w-full h-full origin-top bg-[#FDE4D0] border-b-2 border-[#5C4033] clip-path-triangle"></div>
          </div>
        </div>

        {/* MAIN CARD */}
        <div className="absolute z-50 w-[300px] h-[500px] bg-[#fffaf5] rounded-3xl shadow-2xl overflow-hidden border border-white/40 animate-[float_5s_ease-in-out_infinite]">

          {/* SCRAPBOOK HEADER */}
          <div className="absolute top-5 w-full text-center z-20">
            <h1 className="text-2xl text-black font-light tracking-wide italic drop-shadow-md">
              happy birthday mummum 😭🤍
            </h1>
          </div>

          {/* LEFT LOVE STRIP */}
          <div className="absolute left-0 top-0 h-full w-10 bg-[#d8b89c] flex flex-col items-center justify-center text-[10px] tracking-[3px] text-[#5b4636] uppercase">
            <span className="rotate-[-90deg] whitespace-nowrap">love love love love</span>
          </div>

          {/* HEART BALLOONS */}
          <div className="absolute right-4 top-20 flex flex-col gap-2">
            {[1,2,3,4,5].map((i)=>(
              <div key={i} className="w-7 h-7 bg-red-500 rotate-45 relative animate-bounce rounded-sm">
                <div className="absolute w-7 h-7 bg-red-500 rounded-full -top-3 left-0"></div>
                <div className="absolute w-7 h-7 bg-red-500 rounded-full left-3 top-0"></div>
              </div>
            ))}
          </div>

          {/* POLAROID PHOTOS */}
          <div className="absolute top-28 left-12 rotate-[-8deg] bg-white p-2 shadow-xl w-32 h-40 border">
            <img
              src="https://images.unsplash.com/photo-1517841905240-472988babdf9?q=80&w=800&auto=format&fit=crop"
              className="w-full h-[110px] object-cover"
            />
            <p className="text-center text-xs mt-2 italic">our memories 💖</p>
          </div>

          <div className="absolute top-48 right-10 rotate-[8deg] bg-white p-2 shadow-xl w-32 h-40 border">
            <img
              src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?q=80&w=800&auto=format&fit=crop"
              className="w-full h-[110px] object-cover"
            />
            <p className="text-center text-xs mt-2 italic">forever us ✨</p>
          </div>

          {/* KISS MARKS */}
          <div className="absolute top-32 right-20 text-red-500 text-3xl rotate-12">💋</div>
          <div className="absolute top-60 left-8 text-red-500 text-3xl -rotate-12">💋</div>
          <div className="absolute bottom-36 right-20 text-red-500 text-3xl rotate-6">💋</div>

          {/* SATIN BOW */}
          <div className="absolute top-5 right-5 text-4xl">🎀</div>

          {/* MEMORY FRAME */}
          <div className="absolute bottom-16 left-1/2 -translate-x-1/2 w-[240px] h-[140px] bg-[#2b2b2b] rounded-2xl overflow-hidden border-4 border-white shadow-2xl">

            {/* WASHI TAPE */}
            <div className="absolute top-2 left-2 w-20 h-6 bg-white/40 rotate-[-8deg]"></div>

            {/* IMAGE */}
            <img
              src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?q=80&w=800&auto=format&fit=crop"
              className="w-full h-full object-cover animate-[slideIn_2s_ease]"
            />
          </div>

          {/* STARS */}
          <div className="absolute left-20 bottom-44 text-yellow-500 text-xl">✦</div>
          <div className="absolute right-24 bottom-52 text-yellow-500 text-sm">✦</div>
          <div className="absolute left-10 top-24 text-yellow-500 text-sm">✦</div>

          {/* BOTTOM NOTE */}
          <div className="absolute bottom-3 right-3 bg-[#c8a27d] p-3 rounded-xl shadow-md rotate-[-4deg] w-28">
            <div className="text-red-600 text-2xl">❤</div>
            <p className="text-[10px] mt-1 font-semibold">P.S. I love you!</p>
          </div>

          {/* FLOWERS */}
          <div className="absolute bottom-2 left-4 text-4xl">🌷</div>
        </div>
      </div>

      <style>{`
        .clip-path-triangle {
          clip-path: polygon(0 0, 50% 60%, 100% 0);
        }

        @keyframes slideIn {
          0% {
            transform: translateY(-40px) scale(1.1);
            opacity: 0;
          }
          70% {
            transform: translateY(0px) scale(1);
            opacity: 1;
          }
          85% {
            transform: translateY(4px);
          }
          100% {
            transform: translateY(0px);
          }
        }

        @keyframes float {
          0% {
            transform: translateY(0px);
          }
          50% {
            transform: translateY(-8px);
          }
          100% {
            transform: translateY(0px);
          }
        }
      `}</style>
    </div>
  )
}
