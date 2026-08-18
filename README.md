# Vertix — site institucional

Site estático do **Vertix**, plataforma de gestão para personal trainers:
prescrição de treinos, acompanhamento da execução, avaliação física, frequência,
financeiro e app próprio para o aluno.

🔗 **https://vertix.scobtech.com.br**

---

## Estrutura

```
.
├── index.html          landing em português
├── privacidade.html    Política de Privacidade (LGPD)
├── termos.html         Termos de Uso
├── en/                 versão em inglês (index, privacy, terms)
├── assets/
│   ├── styles.css      folha de estilo única
│   ├── main.js         menu mobile
│   ├── fonts/          Inter e Poppins auto-hospedadas
│   └── *.svg, *.png    logo, ícones e telas do app
├── robots.txt
├── sitemap.xml
└── CNAME               domínio do GitHub Pages
```

## Rodar localmente

Não há build nem dependências. Basta servir a pasta:

```bash
python3 -m http.server 8000
# abra http://localhost:8000
```

## Publicação

Publicado via **GitHub Pages** a partir da branch `main`.
Qualquer push para `main` atualiza o site em poucos minutos.

## Notas técnicas

- HTML, CSS e JavaScript puros — sem framework, sem build, sem dependências.
- **Zero requisições a terceiros:** as fontes são servidas do próprio domínio,
  não há analytics, cookies ou pixels de rastreamento.
- Imagens otimizadas; a home carrega em ~680 KB e 10 requisições.
- Acessibilidade: contraste WCAG AA em todos os pares de cor, `alt` em todas as
  imagens, navegação por teclado com skip link.
- As telas do app exibidas no site usam **dados fictícios**. Nenhum dado de
  aluno real é publicado.

## Licença

Conteúdo, marca e design © Silvio Arruda. Todos os direitos reservados.
