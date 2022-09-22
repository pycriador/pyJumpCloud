## Desafio Loft

O desafio será criar um código em python que:

1. Acesse o google sheets (via API)
2. Recupere os dados do usuários
3. Crie os usuários no JumpCloud (via API) com os dados adquiridos no passo

### Pré-requisitos:

#### Opcional:
* Criar um ambiente virtual Python

<pre>
python -m venv venv
venv\Scripts\activate
</pre>

#### Obrigatório:
* Instalar dependências com pip

<pre>
pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib pandas
</pre>

* Criar uma conta em [https://jumpcloud.com](https://jumpcloud.com)
* Criar ou ter uma conta Google e criar um projeto [https://cloud.google.com](https://cloud.google.com)
* Abrir o arquivo *Resolução Desafio Loft.ipynb* no Google Colab e informar a API Key da JumpCloud e subir via upload a *key.json* baixada do Google Cloud

#### Documentações úteis:

* [JumpCloud API](https://docs.jumpcloud.com/api/2.0/index.html#operation/bulk_usersCreate)
* [Google QuickStart Python](https://developers.google.com/sheets/api/quickstart/python)
* [OAuth 2.0 Server to Server](https://developers.google.com/identity/protocols/oauth2/service-account)
