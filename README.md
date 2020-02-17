## Instalando o Jenkins

Primeiro, adicione a chave do repositório ao sistema:
```
wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -
```

Quando a chave for adicionada, o sistema retornará OK. Em seguida, adicione o endereço do repositório de pacotes Debian ao sources.list do servidor:
```
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
```

Quando ambos estiverem funcionando, execute update para que o apt use o novo repositório:
```
sudo apt update
```

Por fim, instale o Jenkins e suas dependências:
```
sudo apt install jenkins
```

## Configurando o Jenkins

Para configurar sua instalação, visite o Jenkins na sua porta padrão, 8080, usando o nome de domínio ou endereço IP do seu servidor: `http://your_server_ip_or_domain:8080`
