import React from 'react';
import { ShoppingBag, MessageCircle, Star, Truck, ShieldCheck, Menu, X, ChevronRight, Instagram, MapPin, Phone, Mail } from 'lucide-react';

const categories = ['Todos', 'Mais vendidos', 'Novidades', 'Promoções', 'Kits'];

const products = [
  {
    id: 1,
    name: 'WB Collection • Body Desejo Azul',
    category: 'Mais vendidos', collection: 'Noite Proibida',
    price: 'Consulte no WhatsApp',
    description: 'Renda premium com caimento perfeito. Do P ao GG • Cor azul • Elegância e sensualidade.',
    image: '/mnt/data/IMG-20260316-WA0011.jpg',
  },
  {
    id: 2,
    name: 'WB Collection • Duo Bicolor Intense',
    category: 'Novidades', collection: 'Lux Lace',
    price: 'Consulte no WhatsApp',
    description: 'Body bicolor moderno e sensual. Rosa/preto e branco/preto.',
    image: '/mnt/data/IMG-20260316-WA0012.jpg',
  },
  {
    id: 3,
    name: 'WB Collection • Conjunto Tentação',
    category: 'Mais vendidos', collection: 'Noite Proibida',
    price: 'Consulte no WhatsApp',
    description: 'Conjunto rendado em vermelho e preto. Muito procurado 🔥',
    image: '/mnt/data/IMG-20260316-WA0010.jpg',
  },
  {
    id: 4,
    name: 'WB Collection • Body Neon Romance',
    category: 'Novidades', collection: 'Lux Lace',
    price: 'Consulte no WhatsApp',
    description: 'Transparência sofisticada com cores vibrantes.',
    image: '/mnt/data/IMG-20260316-WA0009.jpg',
  },
  {
    id: 5,
    name: 'WB Collection • Body Noite Proibida',
    category: 'Mais vendidos', collection: 'Noite Proibida',
    price: 'Consulte no WhatsApp',
    description: 'Body em renda preto e vermelho com acabamento premium.',
    image: '/mnt/data/IMG-20260316-WA0008.jpg',
  },
  {
    id: 6,
    name: 'WB Collection • Babydoll Soft Desire Branco',
    category: 'Kits', collection: 'Soft Desire',
    price: 'Consulte no WhatsApp',
    description: 'Delicado, leve e elegante. Muito feminino.',
    image: '/mnt/data/IMG-20260312-WA0018.jpg',
  },
  {
    id: 7,
    name: 'WB Collection • Babydoll Soft Desire Preto',
    category: 'Kits', collection: 'Soft Desire',
    price: 'Consulte no WhatsApp',
    description: 'Versão preta com transparência sensual.',
    image: '/mnt/data/IMG-20260312-WA0016.jpg',
  },
  {
    id: 8,
    name: 'WB Collection • Babydoll Rubi Secret',
    category: 'Kits', collection: 'Soft Desire',
    price: 'Consulte no WhatsApp',
    description: 'Babydoll vermelho marcante e sofisticado.',
    image: '/mnt/data/IMG-20260312-WA0014.jpg',
  },
  {
    id: 9,
    name: 'WB Collection • Conjunto Curves Intense Vermelho',
    category: 'Mais vendidos', collection: 'Curves Intense',
    price: 'Consulte no WhatsApp',
    description: 'Plus size com renda e excelente ajuste.',
    image: '/mnt/data/IMG-20260312-WA0013.jpg',
  },
  {
    id: 10,
    name: 'WB Collection • Conjunto Curves Intense Preto',
    category: 'Mais vendidos', collection: 'Curves Intense',
    price: 'Consulte no WhatsApp',
    description: 'Clássico preto sofisticado e sensual.',
    image: '/mnt/data/IMG_20260310_213353_623.jpg',
  },
  {
    id: 11,
    name: 'WB Collection • Conjunto Curves Intense Branco',
    category: 'Mais vendidos', collection: 'Curves Intense',
    price: 'Consulte no WhatsApp',
    description: 'Branco elegante com acabamento premium.',
    image: '/mnt/data/IMG_20260310_213353_814.jpg',
  },
  {
    id: 12,
    name: 'WB Collection • Saia Lux Lace Branco',
    category: 'Novidades', collection: 'Lux Lace',
    price: 'Consulte no WhatsApp',
    description: 'Top rendado com saia translúcida.',
    image: '/mnt/data/IMG_20260310_213353_343.jpg',
  },
  {
    id: 13,
    name: 'WB Collection • Saia Lux Lace Vermelho',
    category: 'Novidades', collection: 'Lux Lace',
    price: 'Consulte no WhatsApp',
    description: 'Conjunto vermelho com presença forte.',
    image: '/mnt/data/IMG_20260310_213353_607.jpg',
  },
  {
    id: 14,
    name: 'WB Collection • Corset Lace Sensation Branco',
    category: 'Promoções', collection: 'Oferta Luxo',
    price: 'Consulte no WhatsApp',
    description: 'Corset com amarração e renda delicada.',
    image: '/mnt/data/IMG_20260310_213353_930.jpg',
  },
  {
    id: 15,
    name: 'WB Collection • Corset Lace Sensation Preto',
    category: 'Promoções', collection: 'Oferta Luxo',
    price: 'Consulte no WhatsApp',
    description: 'Versão preta sofisticada e marcante.',
    image: '/mnt/data/IMG_20260310_213353_641.jpg',
  },
  {
    id: 16,
    name: 'WB Collection • Corset Lace Sensation Vermelho',
    category: 'Promoções', collection: 'Oferta Luxo',
    price: 'Consulte no WhatsApp',
    description: 'Vermelho intenso com alto impacto visual.',
    image: '/mnt/data/IMG_20260310_213353_443.jpg',
  }
];

const testimonials = [
  {
    name: 'Mariana Alves',
    role: 'Cliente recorrente',
    text: 'O site ficou fácil de navegar e eu consegui pedir tudo direto pelo WhatsApp em poucos minutos.',
  },
  {
    name: 'Carlos Henrique',
    role: 'Comprador online',
    text: 'Gostei muito da apresentação dos produtos. Passa confiança e ajuda bastante na escolha.',
  },
  {
    name: 'Fernanda Rocha',
    role: 'Cliente nova',
    text: 'Achei lindo no celular e muito prático para ver os kits e promoções.',
  },
];

const faqs = [
  {
    question: 'Como faço um pedido?',
    answer: 'Você pode selecionar o produto e concluir pelo WhatsApp ou pelo checkout integrado, dependendo da configuração da loja.',
  },
  {
    question: 'Vocês entregam para todo o Brasil?',
    answer: 'Esse modelo já prevê uma área para política de entrega. Depois é só ajustar conforme sua operação.',
  },
  {
    question: 'Posso comprar kits e promoções juntos?',
    answer: 'Sim. O catálogo pode destacar kits, lançamentos e promoções em seções separadas para facilitar a compra.',
  },
];

function Header({ page, setPage }) {
  const [open, setOpen] = React.useState(false);
  const navItems = [
    ['home', 'Início'],
    ['catalogo', 'Catálogo'],
    ['sobre', 'Sobre'],
    ['depoimentos', 'Depoimentos'],
    ['faq', 'FAQ'],
    ['contato', 'Contato'],
  ];

  const handleNav = (nextPage) => {
    setPage(nextPage);
    setOpen(false);
    window.scrollTo({ top: 0, behavior: 'smooth' });
  };

  return (
    <header className="sticky top-0 z-50 border-b border-neutral-200 bg-white/90 backdrop-blur">
      <div className="mx-auto flex max-w-7xl items-center justify-between px-6 py-4 md:px-10">
        <button onClick={() => handleNav('home')} className="text-left">
          <div className="text-lg font-bold tracking-tight">WB Moda & Estilo</div>
          <div className="text-xs text-blue-700/70">Catálogo e vendas online</div>
        </button>

        <nav className="hidden items-center gap-6 md:flex">
          {navItems.map(([key, label]) => (
            <button
              key={key}
              onClick={() => handleNav(key)}
              className={`text-sm font-medium transition ${page === key ? 'text-blue-900' : 'text-blue-700/70 hover:text-blue-900'}`}
            >
              {label}
            </button>
          ))}
        </nav>

        <div className="hidden md:block">
          <a
            href="https://wa.me/5521988247953?text=Oi!%20Quero%20atendimento"
            className="inline-flex items-center gap-2 rounded-2xl bg-blue-900 px-5 py-3 text-sm font-semibold text-white"
          >
            <MessageCircle className="h-4 w-4" />
            Falar no WhatsApp
          </a>
        </div>

        <button onClick={() => setOpen(!open)} className="md:hidden">
          {open ? <X className="h-6 w-6" /> : <Menu className="h-6 w-6" />}
        </button>
      </div>

      {open && (
        <div className="border-t border-neutral-200 bg-white px-6 py-4 md:hidden">
          <div className="flex flex-col gap-3">
            {navItems.map(([key, label]) => (
              <button
                key={key}
                onClick={() => handleNav(key)}
                className="rounded-xl px-3 py-2 text-left text-sm font-medium text-neutral-700 hover:bg-blue-100"
              >
                {label}
              </button>
            ))}
            <a
              href="https://wa.me/5521988247953?text=Oi!%20Quero%20atendimento"
              className="mt-2 inline-flex items-center justify-center gap-2 rounded-2xl bg-blue-900 px-5 py-3 text-sm font-semibold text-white"
            >
              <MessageCircle className="h-4 w-4" />
              Falar no WhatsApp
            </a>
          </div>
        </div>
      )}
    </header>
  );
}

function Hero({ setPage }) {
  return (
    <section className="relative overflow-hidden bg-white">
      <div className="absolute inset-0 bg-gradient-to-br from-blue-100 via-white to-purple-100" />
      <div className="relative mx-auto grid max-w-7xl gap-10 px-6 py-16 md:grid-cols-2 md:px-10 md:py-24">
        <div className="flex flex-col justify-center">
          <span className="inline-flex w-fit rounded-full border border-blue-200 px-4 py-1 text-sm font-medium">
            Wb Lingeries • Coleção Premium
          </span>
          <h1 className="mt-6 text-4xl font-bold tracking-tight md:text-6xl">
            Luxo, sensualidade e desejo em cada detalhe
          </h1>
          <p className="mt-5 max-w-xl text-base leading-7 text-blue-800/80 md:text-lg">
            Estrutura completa com páginas de catálogo, sobre, depoimentos, FAQ e contato. Tudo pronto para adaptar à sua marca e aos seus produtos.
          </p>
          <div className="mt-8 flex flex-wrap gap-4">
            <button
              onClick={() => setPage('catalogo')}
              className="rounded-2xl bg-blue-900 px-6 py-3 text-sm font-semibold text-white shadow-sm"
            >
              Ver catálogo
            </button>
            <button
              onClick={() => setPage('contato')}
              className="rounded-2xl border border-blue-200 bg-white px-6 py-3 text-sm font-semibold text-blue-900 shadow-sm"
            >
              Solicitar atendimento
            </button>
          </div>
        </div>

        <div className="grid gap-4 sm:grid-cols-2">
          <div className="rounded-3xl bg-blue-900 p-6 text-white shadow-xl">
            <p className="text-sm text-neutral-300">Mais conversão</p>
            <p className="mt-3 text-3xl font-bold">Catálogo organizado</p>
            <p className="mt-3 text-sm leading-6 text-neutral-300">
              Coleção exclusiva, promoções e kits para aumentar interesse e vendas.
            </p>
          </div>
          <div className="rounded-3xl bg-white p-6 shadow-xl ring-1 ring-blue-100">
            <p className="text-sm text-blue-700/70">Experiência mobile</p>
            <p className="mt-3 text-3xl font-bold">Feito para celular</p>
            <p className="mt-3 text-sm leading-6 text-blue-800/80">
              Navegação leve e bonita para Instagram, WhatsApp e tráfego pago.
            </p>
          </div>
          <div className="rounded-3xl bg-white p-6 shadow-xl ring-1 ring-blue-100 sm:col-span-2">
            <div className="grid gap-4 md:grid-cols-3">
              <div>
                <div className="flex items-center gap-2 text-sm font-semibold"><Truck className="h-4 w-4" /> Entrega</div>
                <p className="mt-2 text-sm text-blue-800/80">Área pronta para informar prazos e regiões atendidas.</p>
              </div>
              <div>
                <div className="flex items-center gap-2 text-sm font-semibold"><ShieldCheck className="h-4 w-4" /> Confiança</div>
                <p className="mt-2 text-sm text-blue-800/80">Sessões institucionais que reforçam segurança para compra.</p>
              </div>
              <div>
                <div className="flex items-center gap-2 text-sm font-semibold"><ShoppingBag className="h-4 w-4" /> Conversão</div>
                <p className="mt-2 text-sm text-blue-800/80">Botões de ação pensados para facilitar orçamento e pedido.</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      {/* Botão flutuante WhatsApp */}
      <a
        href="https://wa.me/5521988247953?text=Oi! Quero atendimento 😊"
        className="fixed bottom-5 right-5 z-50 rounded-full bg-green-500 px-5 py-3 text-sm font-semibold text-white shadow-lg hover:scale-105 transition"
      >
        💬 Falar no WhatsApp
      </a>

    </section>
  );
}

function HomePage({ setPage }) {
  return (
    <>
      <Hero setPage={setPage} />

      <section className="mx-auto max-w-7xl px-6 py-14 md:px-10">
        <div className="grid gap-6 md:grid-cols-3">
          {[
            ['Catálogo inteligente', 'Produtos separados por categorias, destaques e busca rápida.'],
            ['Página institucional', 'Conte sua história, mostre diferenciais e gere confiança.'],
            ['Contato facilitado', 'Links para WhatsApp, redes sociais, formulário e localização.'],
          ].map(([title, text]) => (
            <div key={title} className="rounded-3xl bg-white p-6 shadow-sm ring-1 ring-blue-100">
              <h3 className="text-xl font-semibold">{title}</h3>
              <p className="mt-3 text-sm leading-6 text-blue-800/80">{text}</p>
            </div>
          ))}
        </div>
      </section>

      <section className="mx-auto max-w-7xl px-6 pb-16 md:px-10">
        <div className="rounded-[2rem] bg-blue-900 px-8 py-10 text-white md:px-12 md:py-14">
          <div className="grid gap-8 md:grid-cols-2 md:items-center">
            <div>
              <h3 className="text-3xl font-bold tracking-tight">Estrutura pronta para virar seu site real</h3>
              <p className="mt-3 max-w-xl text-neutral-300">
                Basta trocar nome da marca, identidade visual, produtos, links, depoimentos e informações de contato.
              </p>
            </div>
            <div className="flex flex-wrap gap-4 md:justify-end">
              <button
                onClick={() => setPage('sobre')}
                className="rounded-2xl bg-white px-6 py-3 text-sm font-semibold text-blue-900"
              >
                Conhecer a marca
              </button>
              <button
                onClick={() => setPage('contato')}
                className="rounded-2xl border border-white/20 px-6 py-3 text-sm font-semibold text-white"
              >
                Ir para contato
              </button>
            </div>
          </div>
        </div>
      </section>
    </>
  );
}

function CatalogPage() {
  const [selectedCategory, setSelectedCategory] = React.useState('Todos');
  const [search, setSearch] = React.useState('');

  const filteredProducts = products.filter((product) => {
    const categoryMatch = selectedCategory === 'Todos' || product.category === selectedCategory;
    const searchMatch = `${product.name} ${product.description}`.toLowerCase().includes(search.toLowerCase());
    return categoryMatch && searchMatch;
  });

  return (
    <section className="mx-auto max-w-7xl px-6 py-14 md:px-10">
      <div className="flex flex-col gap-5 md:flex-row md:items-end md:justify-between">
        <div>
          <p className="text-sm font-medium text-blue-700/70">Página de catálogo</p>
          <h2 className="mt-2 text-3xl font-bold tracking-tight">Coleção WB • Destaques</h2>
          <p className="mt-2 text-blue-800/80">Explore a coleção WB, descubra peças exclusivas e fale direto no WhatsApp para garantir a sua.</p>
        </div>

        <div className="flex w-full flex-col gap-3 md:max-w-xl">
          <input
            value={search}
            onChange={(e) => setSearch(e.target.value)}
            placeholder="Buscar produto"
            className="w-full rounded-2xl border border-blue-200 bg-white px-4 py-3 outline-none transition focus:border-neutral-500"
          />
          <div className="flex flex-wrap gap-2">
            {categories.map((category) => (
              <button
                key={category}
                onClick={() => setSelectedCategory(category)}
                className={`rounded-full px-4 py-2 text-sm font-medium transition ${
                  selectedCategory === category ? 'bg-blue-900 text-white' : 'bg-white text-neutral-700 ring-1 ring-neutral-300'
                }`}
              >
                {category}
              </button>
            ))}
          </div>
        </div>
      </div>

      <div className="mt-10 grid gap-6 md:grid-cols-2 xl:grid-cols-3">
        {filteredProducts.map((product) => (
          <article key={product.id} className="group overflow-hidden rounded-3xl bg-white shadow-sm ring-1 ring-blue-100 transition hover:-translate-y-1 hover:shadow-xl">
            <div className="aspect-[4/3] overflow-hidden relative">
              {product.category === 'Mais vendidos' && (
                <span className="absolute left-3 top-3 z-10 rounded-full bg-red-500 px-3 py-1 text-xs font-semibold text-white">🔥 Mais vendido</span>
              )}
              {product.category === 'Promoções' && (
                <span className="absolute right-3 top-3 z-10 rounded-full bg-purple-600 px-3 py-1 text-xs font-semibold text-white">💥 Oferta</span>
              )}
              {product.category === 'Novidades' && (
                <span className="absolute left-3 bottom-3 z-10 rounded-full bg-blue-600 px-3 py-1 text-xs font-semibold text-white">✨ Novo</span>
              )}
              <img src={product.image} alt={product.name} className="h-full w-full object-cover transition duration-300 group-hover:scale-105" />
            </div>
            <div className="p-5">
              <p className="text-sm text-blue-700/70">{product.category} • {product.collection}</p>
              <h3 className="mt-1 text-xl font-semibold">{product.name}</h3>
              <p className="mt-3 text-sm leading-6 text-blue-800/80">{product.description}</p>
              <div className="mt-5 flex flex-col gap-2">
                <span className="text-lg font-bold">{product.price}</span>
                <a
                  href={`https://wa.me/5521988247953?text=${encodeURIComponent(`Oi! Vi esse produto no site (${product.name}) e quero saber o preço e disponibilidade 😊`)}`}
                  className="inline-flex items-center justify-center gap-2 rounded-2xl bg-blue-900 px-4 py-3 text-sm font-semibold text-white"
                >
                  💬 Quero saber o preço <ChevronRight className="h-4 w-4" />
                </a>
                <span className="text-xs text-blue-700/70 text-center">💬 Atendimento rápido no WhatsApp</span>
              </div>
            </div>
          </article>
        ))}
      </div>
    </section>
  );
}

function AboutPage() {
  return (
    <section className="mx-auto max-w-7xl px-6 py-14 md:px-10">
      <div className="grid gap-10 md:grid-cols-2 md:items-center">
        <div>
          <p className="text-sm font-medium text-blue-700/70">Página sobre</p>
          <h2 className="mt-2 text-3xl font-bold tracking-tight">Apresente sua marca com mais valor</h2>
          <p className="mt-4 text-base leading-7 text-blue-800/80">
            Essa seção foi pensada para contar a história da empresa, mostrar o propósito da marca e reforçar diferenciais competitivos. Em um site de vendas, isso ajuda a construir confiança e melhorar a tomada de decisão do cliente.
          </p>
          <div className="mt-8 grid gap-4 sm:grid-cols-2">
            {[
              'Atendimento próximo e humanizado',
              'Produtos selecionados com curadoria',
              'Experiência simples no celular',
              'Comunicação clara para vender mais',
            ].map((item) => (
              <div key={item} className="rounded-2xl bg-white p-4 shadow-sm ring-1 ring-blue-100">
                <div className="flex items-start gap-3">
                  <Star className="mt-0.5 h-5 w-5" />
                  <p className="text-sm font-medium text-neutral-700">{item}</p>
                </div>
              </div>
            ))}
          </div>
        </div>

        <div className="overflow-hidden rounded-[2rem] bg-white shadow-xl ring-1 ring-blue-100">
          <img
            src="https://images.unsplash.com/photo-1520607162513-77705c0f0d4a?auto=format&fit=crop&w=1200&q=80"
            alt="Equipe e marca"
            className="h-full w-full object-cover"
          />
        </div>
      </div>
    </section>
  );
}

function TestimonialsPage() {
  return (
    <section className="mx-auto max-w-7xl px-6 py-14 md:px-10">
      <p className="text-sm font-medium text-blue-700/70">Página de depoimentos</p>
      <h2 className="mt-2 text-3xl font-bold tracking-tight">O que os clientes dizem</h2>
      <div className="mt-10 grid gap-6 md:grid-cols-3">
        {testimonials.map((testimonial) => (
          <div key={testimonial.name} className="rounded-3xl bg-white p-6 shadow-sm ring-1 ring-blue-100">
            <div className="mb-4 flex gap-1">
              {[...Array(5)].map((_, i) => (
                <Star key={i} className="h-4 w-4 fill-current" />
              ))}
            </div>
            <p className="text-sm leading-6 text-blue-800/80">“{testimonial.text}”</p>
            <div className="mt-5">
              <p className="font-semibold">{testimonial.name}</p>
              <p className="text-sm text-blue-700/70">{testimonial.role}</p>
            </div>
          </div>
        ))}
      </div>
    </section>
  );
}

function FaqPage() {
  const [openIndex, setOpenIndex] = React.useState(0);

  return (
    <section className="mx-auto max-w-4xl px-6 py-14 md:px-10">
      <p className="text-sm font-medium text-blue-700/70">Página FAQ</p>
      <h2 className="mt-2 text-3xl font-bold tracking-tight">Perguntas frequentes</h2>
      <div className="mt-10 space-y-4">
        {faqs.map((faq, index) => {
          const open = openIndex === index;
          return (
            <div key={faq.question} className="overflow-hidden rounded-3xl bg-white shadow-sm ring-1 ring-blue-100">
              <button
                onClick={() => setOpenIndex(open ? -1 : index)}
                className="flex w-full items-center justify-between gap-4 px-6 py-5 text-left"
              >
                <span className="font-semibold">{faq.question}</span>
                <span className="text-xl">{open ? '−' : '+'}</span>
              </button>
              {open && <div className="px-6 pb-6 text-sm leading-6 text-blue-800/80">{faq.answer}</div>}
            </div>
          );
        })}
      </div>
    </section>
  );
}

function ContactPage() {
  return (
    <section className="mx-auto max-w-7xl px-6 py-14 md:px-10">
      <div className="grid gap-8 md:grid-cols-2">
        <div>
          <p className="text-sm font-medium text-blue-700/70">Página de contato</p>
          <h2 className="mt-2 text-3xl font-bold tracking-tight">Atendimento exclusivo WB</h2>
          <p className="mt-4 max-w-xl text-base leading-7 text-blue-800/80">
            Deixe aqui os canais principais de atendimento, localização, horário de funcionamento e redes sociais. Isso completa o site e melhora a confiança do cliente.
          </p>

          <div className="mt-8 space-y-4">
            <div className="flex items-start gap-3 rounded-2xl bg-white p-4 shadow-sm ring-1 ring-blue-100">
              <Phone className="mt-0.5 h-5 w-5" />
              <div>
                <p className="font-semibold">WhatsApp</p>
                <p className="text-sm text-blue-800/80">(21) 98824-7953</p>
              </div>
            </div>
            <div className="flex items-start gap-3 rounded-2xl bg-white p-4 shadow-sm ring-1 ring-blue-100">
              <Mail className="mt-0.5 h-5 w-5" />
              <div>
                <p className="font-semibold">E-mail</p>
                <p className="text-sm text-blue-800/80">contato@wblingeries.com</p>
              </div>
            </div>
            <div className="flex items-start gap-3 rounded-2xl bg-white p-4 shadow-sm ring-1 ring-blue-100">
              <MapPin className="mt-0.5 h-5 w-5" />
              <div>
                <p className="font-semibold">Endereço</p>
                <p className="text-sm text-blue-800/80">Rio de Janeiro - RJ</p>
              </div>
            </div>
          </div>
        </div>

        <div className="rounded-[2rem] bg-white p-6 shadow-sm ring-1 ring-blue-100 md:p-8">
          <h3 className="text-xl font-semibold">Solicite atendimento</h3>
          <div className="mt-6 grid gap-4">
            <input placeholder="Seu nome" className="rounded-2xl border border-blue-200 px-4 py-3 outline-none focus:border-neutral-500" />
            <input placeholder="Seu WhatsApp" className="rounded-2xl border border-blue-200 px-4 py-3 outline-none focus:border-neutral-500" />
            <input placeholder="Seu e-mail" className="rounded-2xl border border-blue-200 px-4 py-3 outline-none focus:border-neutral-500" />
            <textarea placeholder="Como podemos ajudar?" rows={5} className="rounded-2xl border border-blue-200 px-4 py-3 outline-none focus:border-neutral-500" />
            <a
              href="https://wa.me/5521988247953?text=Oi!%20Quero%20atendimento"
              className="inline-flex items-center justify-center gap-2 rounded-2xl bg-blue-900 px-6 py-3 text-sm font-semibold text-white"
            >
              <MessageCircle className="h-4 w-4" />
              Enviar para WhatsApp
            </a>
          </div>
        </div>
      </div>
    </section>
  );
}

function Footer({ setPage }) {
  return (
    <footer className="border-t border-neutral-200 bg-white">
      <div className="mx-auto grid max-w-7xl gap-8 px-6 py-10 md:grid-cols-4 md:px-10">
        <div>
          <h4 className="text-lg font-bold">WB Moda & Estilo</h4>
          <p className="mt-3 text-sm leading-6 text-blue-800/80">
            Modelo de site completo para catálogo, vendas e atendimento.
          </p>
        </div>
        <div>
          <h5 className="font-semibold">Páginas</h5>
          <div className="mt-3 flex flex-col gap-2 text-sm text-blue-800/80">
            {[
              ['home', 'Início'],
              ['catalogo', 'Catálogo'],
              ['sobre', 'Sobre'],
              ['contato', 'Contato'],
            ].map(([key, label]) => (
              <button key={key} onClick={() => setPage(key)} className="text-left hover:text-blue-900">
                {label}
              </button>
            ))}
          </div>
        </div>
        <div>
          <h5 className="font-semibold">Contato</h5>
          <div className="mt-3 space-y-2 text-sm text-blue-800/80">
            <p>(21) 98824-7953</p>
            <p>contato@wblingeries.com</p>
            <p>Atendimento online - Rio de Janeiro</p>
          </div>
        </div>
        <div>
          <h5 className="font-semibold">Redes sociais</h5>
          <div className="mt-3 flex gap-3 text-blue-800/80">
            <a href="https://instagram.com/wblingerieesexshop" className="rounded-full border border-blue-200 p-2"><Instagram className="h-4 w-4" /></a>
            <a href="https://wa.me/5521988247953" className="rounded-full border border-blue-200 p-2"><MessageCircle className="h-4 w-4" /></a>
          </div>
        </div>
      </div>
    </footer>
  );
}

export default function CatalogoVendasSite() {
  const [page, setPage] = React.useState('home');

  return (
    <div className="min-h-screen bg-blue-50 text-blue-900">
      <Header page={page} setPage={setPage} />

      {page === 'home' && <HomePage setPage={setPage} />}
      {page === 'catalogo' && <CatalogPage />}
      {page === 'sobre' && <AboutPage />}
      {page === 'depoimentos' && <TestimonialsPage />}
      {page === 'faq' && <FaqPage />}
      {page === 'contato' && <ContactPage />}

      <Footer setPage={setPage} />
    </div>
  );
}
