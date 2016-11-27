```javascript
{
    "key": "value",
    "nome": "Pedro",
    "idade": 28,
    "ps4": true,
}
```
---
```html
<html>
<body>
  <form action="/usuario" method="post">
    <input type="text" value="nome">
    <input type="text" value="idade">
    <input type="text" value="ps4">
    <input type="submit" value="vai la filhao">
  </form>
</body>
</html>
```
---
```javascript
app.post('/usuario',function(req,res){
  let novoUsuario = req.body;
  console.log(novoUsuario.nome);
  console.log(novoUsuario.idade);
  console.log(novoUsuario.ps4);

  res.status(200).json({status:'ok'})
  });
```
---
```javascript
/*
lista http status
200 = ok
204 = ok, sem conteudo

404 = not found

500 = pau no servidor
503 = pau no servidor
505 = pau no servidor

403 = acesso ñ permitido
405 = acesso negado
*/
```
