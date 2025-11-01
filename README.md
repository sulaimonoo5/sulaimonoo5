![banner](https://capsule-render.vercel.app/api?text=Welcome!&animation=fadeIn&type=waving&color=gradient&height=100)


<card>
export default function AboutMe() {
  const info = [
    { icon: "👂", text: "My name is", value: "Sulaymon Jonmahmadzoda" },
    { icon: "🔭", text: "I’m currently working on", value: "a multi-chat AI project" },
    { icon: "🌱", text: "I’m currently learning", value: "React & Tailwind CSS" },
    { icon: "🤝", text: "I’m looking to collaborate on", value: "frontend and AI tools" },
    { icon: "💬", text: "Ask me about", value: "JavaScript, Tailwind, and UI design" },
    { icon: "📫", text: "How to reach me", value: (
        <>
          <a href="https://t.me/yourhandle" className="text-blue-500 hover:underline">Telegram</a> |{" "}
          <a href="mailto:you@example.com" className="text-blue-500 hover:underline">Email</a>
        </>
      )
    },
    { icon: "❤️", text: "I love", value: "creating modern web experiences" },
    { icon: "⚡", text: "Fun fact", value: "I always refactor my code before sleeping 😄" },
  ];

  return (
    <section className="max-w-xl mx-auto py-10">
      <h2 className="text-3xl font-bold mb-6 text-center">Hi there 👋</h2>
      <ul className="space-y-3 text-lg">
        {info.map((item, i) => (
          <li key={i}>
            <span className="mr-2">{item.icon}</span>
            <strong>{item.text}</strong>: {item.value}
          </li>
        ))}
      </ul>
    </section>
  );
}
</card>
