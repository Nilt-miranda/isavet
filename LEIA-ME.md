# Site — Dra. Isabelle Sudario

Site de página única, pronto pra publicar. Tudo em um arquivo: `index.html`.

## O que você precisa fazer (3 passos)

### 1. Adicionar as fotos
Coloque as imagens na pasta `assets/` com estes nomes:

- `assets/isabelle.png` → foto do **hero** (aquela dela abraçando o filhote, de fundo transparente, fica perfeita)
- `assets/isabelle-sobre.jpg` → foto da seção **Sobre**

> Enquanto não colocar, o site mostra um espaço "Adicione a foto" no lugar — não quebra.

### 2. Configurar WhatsApp e Agenda
Abra o `index.html`, vá até o final no bloco **CONFIGURAÇÃO** e edite:

```js
const CONFIG = {
  whatsapp: "5511999999999",   // 55 + DDD + número (só dígitos)
  whatsappMsg: "Olá, Dra. Isabelle! ...",
  agendaEmbedUrl: ""           // (opcional) embutir a agenda do Google na página
};
```

Por padrão o agendamento é pelo **WhatsApp** (um único botão).

**Mostrar a agenda do Google dentro do site (opcional):** no Google Calendar da Dra., crie um *"Cronograma de agendamentos"* (Appointment schedule) → **Compartilhar/Incorporar** → copie o valor de `src="..."` do iframe e cole em `agendaEmbedUrl`. A agenda aparece ao lado do botão automaticamente.

### 3. Publicar (grátis)
- **Netlify:** arraste a pasta `isavet` inteira em app.netlify.com/drop
- **Vercel** ou **GitHub Pages** também funcionam (é só HTML estático).

## Ver localmente
Abrir o `index.html` direto no navegador já funciona. Ou rode um servidor:
```
python -m http.server 8770
```
e acesse http://localhost:8770
