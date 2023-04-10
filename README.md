
<h1><li>Pata Amiga</li></h1>
<h4> Nosso aplicativo é voltado para adoção de Pets, você pode doar e também adotar um Pet, de maneira rápida e simples.</h4>

<h1><li>Membros</li></h1>
<ol>
    <li><strong>Matheus Victor</strong> - Matrícula: 01515370</li>
    <li> <strong>Everton Figueirôa</strong> - Matrícula: 01177129 </li>
</ol>
<h1>
    <li>
        UML do BackEnd
    </li>
</h1>
<img src="https://user-images.githubusercontent.com/103688000/230797530-6a6b8f8e-ffc8-4d51-b574-df38fa23bcd1.png"/>
<h1>
    <li>
        UML do mobile
    </li>
</h1>
<img src="https://user-images.githubusercontent.com/103688000/230797836-92af65aa-b379-44d9-a904-c02d6f17bdf7.png"/>

<h1><li>Imagens do Projeto - Figma</li></h1>

 <h2>Splash Screen / Tela de Inicial</h2>

![Splash screen](https://user-images.githubusercontent.com/110360268/230796788-f2f86f81-df93-43ad-819a-5c46e2eddc07.png)
![Login](https://user-images.githubusercontent.com/110360268/230796904-b636fa93-ec2e-4018-818f-dd78130c6da8.png)

<h2> Tela de Login </h2>

![Login Screen](https://user-images.githubusercontent.com/110360268/230796914-961c90e2-a794-49ab-be20-c751ebcf3de4.png)

<h2> Tela de Cadastro </h2>

![Register Part 1](https://user-images.githubusercontent.com/110360268/230796936-23effc62-40d8-4821-9421-5535bce4011f.png)
![Register Part 2](https://user-images.githubusercontent.com/110360268/230796938-57828338-c894-471f-a194-4adc28d0a2ea.png)

<h2> Tela Principal </h2>

![Home](https://user-images.githubusercontent.com/110360268/230796921-e5cc867f-c303-40c4-adb3-9ae6152d5c34.png)

<h2> Tela do Perfil do Pet </h2>

![Pet Profile](https://user-images.githubusercontent.com/110360268/230796985-a42275ac-a115-4c96-8812-93425a31ead6.png)

<h2> Tela de para aplicar Filtro na Pesquisa </h2>

![Filter](https://user-images.githubusercontent.com/110360268/230796975-239850e8-f55c-4b30-af8d-f115c44a8327.png)

<h2> Tela para adicionar um Pet para adoção </h2>

![New Animal](https://user-images.githubusercontent.com/110360268/230796980-c09d1af2-dddf-4ecc-8f5a-19319cfe402c.png)

<h2> Tela para edição do Perfil do Usuário </h2>

![Profile Editing](https://user-images.githubusercontent.com/110360268/230796990-dd6e2f87-6c51-4e6d-a008-0cde96589754.png)

<h1>
    <li> 
        Requisitos do Sistema 
    </li>
</h1>
<h4>Requisitos funcionais</h4>

<h1>JSON</h1>
<h2>EndPoints da API</h2>

<h3>Login</h3>

```Post```


<h4>/user/login</h4>
<strong>Body:</strong>

```ruby
{
    "email": String,
    "password": String,
}
```

<h4>
    Return:
</h4>

```status code:``` 200 ```ok```

```
{
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ"
}
```

<h3>CreateUser</h3>

```Post```


<h4>/user</h4>
<strong>Body:</strong>

```ruby
{
    "id": Long,
    "email": String,
    "name": String,
    "password": String,
    "birth": String,
    "location": String,
    "profileAvatarUrl": String,
    "phone": String,
    "socialMidia?": {
        "instagram?": String,
        "facebook?": String,
    }
}
```

<h4>
    Return:
</h4>

```status code:``` 201 ```created```


<h3>getOneUser</h3>

```get```


<h4>/user/{idUser}</h4>


<h4>
    Return:
</h4>


```ruby
{
    "id": Long,
    "email": String,
    "name": String,
    "birth": String,
    "location": String,
    "profileAvatarUrl": String,
    "phone": String,
    "socialMidia?": {
        "instagram?": String,
        "facebook?": String,
    }
}
```

```status code:``` 200 ```OK```


<h3>updateUser</h3>

```patch```

<h4>/user/{idUser}</h4>
<strong>Body:</strong>


```ruby
{
    "id": Long,
    "email": String,
    "name": String,
    "password": String,
    "birth": String,
    "location": String,
    "profileAvatarUrl": String,
    "phone": String,
    "socialMidia?": {
        "instagram?": String,
        "facebook?": String,
    }
}
```

<h4>
    Return:
</h4>

```status code:``` 200 ```OK```
