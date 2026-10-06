# Apoio Psicológico

## Requisitos
- Node.js 18 ou mais novo
- MySQL rodando na sua máquina

## Passo a passo
1. Abra um terminal nesta pasta.
2. `npm install`
3. Se o seu MySQL tem senha no usuário root, defina antes (Windows PowerShell: `$env:DB_PASS="sua_senha"`; Mac/Linux: `export DB_PASS=sua_senha`).
4. `npm run setup`   (cria o banco, as tabelas e as contas de teste)
5. `npm start`
6. Abra http://localhost:3000/login.html

## Contas de teste
| Perfil | E-mail | Senha |
|---|---|---|
| Administrador | admin@teste.com | Admin123! |
| Psicólogo | psi@teste.com | Psi12345 |
| Usuário | user@teste.com | User1234 |

## Estrutura
- public/  telas (HTML, CSS, JS)
- api/     servidor Node e schema.sql
- setup.js cria o banco e os dados de teste

Variáveis opcionais: DB_HOST, DB_USER, DB_PASS, JWT_SECRET.
