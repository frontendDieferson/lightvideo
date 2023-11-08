# Aplicação de compressão de vídeos com Flask REST API e ReactJS

### Descrição:

Este projeto demonstra como criar uma aplicação de compressão de vídeos usando Flask REST API e ReactJS.

A aplicação usa um algoritmo de compressão simples que reduz a resolução e a taxa de quadros do vídeo.

A aplicação também suporta armazenamento temporário de vídeos comprimidos no Firebase Storage com um prazo de 7 dias para serem baixados.

### Requisitos:

Python 3.7+
Flask
ReactJS
Firebase
Instalação:

Clone o repositório
git clone https://github.com/frontendDieferson/lightvideo

### Crie um ambiente virtual
```
python3 -m venv venv
```

### Ative o ambiente virtual
```
source venv/bin/activate
```
### Instale as dependências
```
pip install -r requirements.txt
```

### Configurando o Firebase:

Crie um projeto no Firebase

Habilite o serviço Firebase Storage

Obtenha as credenciais do seu projeto

Crie um arquivo .env na pasta raiz do projeto e adicione as seguintes variáveis de ambiente:

`FIREBASE_API_KEY="[sua-api-key]"`
`FIREBASE_AUTH_DOMAIN="[seu-auth-domain]"`
`FIREBASE_DATABASE_URL="[seu-database-url]"`
`FIREBASE_PROJECT_ID="[seu-project-id]"`
`FIREBASE_STORAGE_BUCKET="[seu-bucket-de-armazenamento]"`

### Execução da aplicação:

Inicie o servidor Flask

```
flask run
```

Abra o navegador e acesse http://localhost:5000
Uso da aplicação:

Clique no botão Selecionar arquivo para selecionar o arquivo de vídeo que deseja compactar.

Clique no botão Comprimir e enviar para compactar o vídeo e enviá-lo para o Firebase Storage.

O vídeo comprimido estará disponível para download na pasta compressed_videos do bucket de armazenamento [seu-bucket-de-armazenamento].

Dicas para melhorar a qualidade da compressão de vídeo:

Use um algoritmo de compressão de vídeo mais eficiente.
Use técnicas de redução de ruído para melhorar a qualidade do vídeo comprimido.
Use técnicas de codificação de perdas para reduzir ainda mais o tamanho do vídeo comprimido.

### Futuros desenvolvimentos:

 - Adicionar suporte para diferentes formatos de vídeo.
- Adicionar suporte para diferentes algoritmos de compressão.
- Adicionar suporte para técnicas de redução de ruído.
- Adicionar suporte para técnicas de codificação de perdas.
- Adicionar suporte para controle de qualidade.
- Adicionar suporte para armazenamento em nuvem.