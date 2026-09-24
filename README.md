# Mi Modas Feminina

Site estático (HTML/CSS/JS puro, sem build) pronto para subir no Vercel via Git.

## Como colocar no ar

### 1. Suba os arquivos para o GitHub
```bash
git init
git add .
git commit -m "Primeira versão do site Mi Modas Feminina"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/mi-modas.git
git push -u origin main
```
(Crie antes um repositório vazio no GitHub com esse nome.)

### 2. Conecte no Vercel
1. Acesse https://vercel.com e faça login (pode usar sua conta do GitHub).
2. Clique em **Add New → Project**.
3. Selecione o repositório que você acabou de subir.
4. Em **Framework Preset**, deixe como **Other** (é um site estático).
5. Não precisa configurar Build Command nem Output Directory — o `index.html` já está na raiz.
6. Clique em **Deploy**.

Em cerca de 1 minuto o Vercel gera um link (algo como `mi-modas.vercel.app`).

## Importante sobre os dados

O "banco de dados" (usuários, produtos e pedidos) fica salvo no `localStorage` do navegador de cada visitante — não é um banco compartilhado entre pessoas ou dispositivos. Isso significa:
- Cada cliente só vê os próprios pedidos, no próprio navegador.
- Produtos cadastrados pelo admin em um navegador não aparecem automaticamente em outro.

Para uma loja de verdade, com produtos e pedidos compartilhados entre todos os visitantes, o próximo passo é conectar um banco de dados real (ex: Supabase, Firebase ou Postgres) — posso te ajudar a planejar isso quando quiser evoluir o site.

## Conta de teste do lojista
- E-mail: `admin@loja.com`
- Senha: `admin123`
