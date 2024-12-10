

## Página Principal

Para criar a página principal, criamos o [layout.js](../src/app/layout.js) e o [page.js](../src/app/page.js), padrão do Next.js 14 (framework utilizado no projeto). E na página `page.js`, temos uma arquitetura baseada em componentes, como você pode ver aqui:

```js
export default function Home() {
  return (
    <main className="flex min-h-screen flex-col bg-[#ffffffff]">
      <Navbar /> // componente Navbar
      <div className="container mt-24 mx-auto px-12 py-4">
        <HeroSection />  // início dos componentes
        <AchievementsSection />
        <AboutSection />
        <ProjectsSection />
        <EmailSection /> // fim dos componentes
      </div>
      <Footer /> // componente Footer
    </main>
  );
}
```

Agora veja o componente de layout, que é utilizado apenas para renderizar o `page.js`:

```js
export default function RootLayout({ children }) {
  return (
    <html lang="en">
      <body className={inter.className}>{children}</body>
    </html>
  )
}
```

## Componentes usados no código:

```
Clique no link para ver a documentação de cada componente
```

* [Navbar](../Components/Navbar.md)
* [HeroSection](../Components/heroSection.md)
* [AchivementsSection](../Components/AchivementsSection.md)
* [AboutSection](../Components/AboutSection.md)
* [ProjectsSection](../Components/ProjectsSection.md)
* [EmailSection](../Components/EmailSection.md)
* [Footer](../Components/Footer.md)

[Voltar para o Índice ⏎](../Index.md)

--- 
