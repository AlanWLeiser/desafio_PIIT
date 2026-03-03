# Desafio Técnico Seleção PIIT: MVP SDGA (Sistema Dinâmico de Gestão de Ativos)
## O Contexto 
Imagine o seguinte cenário: é sexta-feira, o setor de Marketing da instituição precisa gravar um podcast urgente e a Câmera Sony Alpha sumiu. Depois de muita caçada, descobrem que o setor de Eventos pegou a câmera emprestada, mas ninguém anotou em lugar nenhum. 

O problema é claro: falta de controle e visibilidade em tempo real dos ativos.

## A Sua Missão
Sua tarefa como Desenvolvedor(a) Front-end neste desafio é criar a primeira versão (MVP) de um painel de controle para resolver essa bagunça.

Você vai desenvolver uma Single Page Application (SPA) em React que simule o painel de disponibilidade de equipamentos e espaços. O usuário precisa entrar na tela, ver o que está disponível e conseguir "reservar" o item com um clique.

## O que você deve desenvolver (Requisitos Mínimos)
Consumo de Dados: Fazer uma requisição GET para uma API (forneceremos o mock) e listar todos os ativos disponíveis na tela.

Interface (UI): Renderizar esses itens em formato de Cards ou em uma Tabela amigável. Cada item deve exibir:

- Nome do Ativo
- Categoria (ex: Audiovisual, Espaço, Esporte)
- Status Atual (`Disponível` ou `Reservado`)

Interatividade (UX): Para cada item com status `Disponível`, deve existir um botão de `Reservar`.

Gerenciamento de Estado: Ao clicar em `Reservar`, o status do item deve mudar imediatamente na interface para `Reservado` e o botão deve ser desabilitado ou mudar de cor (tudo isso gerenciado no estado do React, não precisa persistir no banco de dados real neste momento).

Tratamento de Fluxo: Exibir um "Carregando..." enquanto os dados da API não chegam na tela.

### Formato da API (Mock)
Você deve basear o seu desenvolvimento na seguinte estrutura de dados. (Dica: você pode usar o json-server ou colocar esse JSON estático no seu código para simular a requisição fetch inicial).

```JSON
[
  {
    "id": 1,
    "nome": "Câmera Sony Alpha a7 III",
    "categoria": "Audiovisual",
    "status": "Disponível",
    "imagem_url": "https://via.placeholder.com/150"
  },
  {
    "id": 2,
    "nome": "Sala de Estudos 04 - Biblioteca",
    "categoria": "Espaço Físico",
    "status": "Reservado",
    "imagem_url": "https://via.placeholder.com/150"
  },
  {
    "id": 3,
    "nome": "Microfone de Lapela Rode Wireless",
    "categoria": "Audiovisual",
    "status": "Disponível",
    "imagem_url": "https://via.placeholder.com/150"
  },
  {
    "id": 4,
    "nome": "Projetor Epson Sala Multiuso",
    "categoria": "Equipamento Didático",
    "status": "Disponível",
    "imagem_url": "https://via.placeholder.com/150"
  }
]
```

## Entregáveis e Diferenciais de Mercado
### Obrigatório:

- Entrega até 10/03/2026
 
- O código deve ser entregue em um repositório público no GitHub.

- O README.md deve conter o passo a passo exato de como rodar o seu projeto localmente (ex: npm install, npm run dev).

### O que vai fazer seu perfil brilhar (Diferenciais):

- Projeto criado utilizando Vite.

- Uso de TypeScript para tipagem dos dados do ativo.

- Aplicação rodando online (Deploy gratuito na Vercel, Netlify ou similar).

- Uma interface limpa e responsiva.
