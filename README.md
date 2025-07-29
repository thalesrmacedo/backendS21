**Passo 1 - Registrar um Usuário**
Método: POST
URL: http://127.0.0.1:5000/register
Aba: Body → raw → JSON

{
  "username": "nomedoaluno",
  "password": "1234"
}

----------------------------------
**Passo 2 - Login para obter o Token**
Método: POST
URL: http://127.0.0.1:5000/login
Aba: Body → raw → JSON

{
  "username": "nomedoaluno",
  "password": "1234"
}

Vai gerar um token, copiar sem as aspas e sem as chaves

----------------------------------
**Passo 3 - Acessar a Rota Protegida**

Método: GET
URL: http://127.0.0.1:5000/protegido
Aba: Authorization

Tipo: Bearer Token

Cole o token no campo (sem as aspas e sem as chaves)
