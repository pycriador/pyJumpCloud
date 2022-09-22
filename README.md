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

## Criando JSON no Google Cloud

Logar no Google, acessar [https://cloud.google.com](https://cloud.google.com), entrar no console e criar projeto:

![Criar projeto](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Criar%20projeto.PNG)

![Novo Projeto](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Novo%20Projeto.PNG)

Em "APIs e Serviços"
![API e Serviços](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/API%20e%20Servi%C3%A7os.PNG)

Clicar em "+ ATIVAR APIS E SERVIÇOS"
![Ativar APIS](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Ativar%20API%20e%20Servi%C3%A7os.PNG)

Procurar Google Sheets e Ativar
![Procurar Google Sheets](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Procurar%20Google%20Sheets%20API.PNG)

Criar credenciais
![Criar credenciais](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Criar%20Credenciais%20Google%20Sheets.PNG)

![Criar credenciais P1](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Tipo%20de%20credencial.PNG)

![Criar credenciais P2](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Tipo%20de%20credencial%20P2.PNG)

Adicionar detalhes do serviço
![Detalhes do Serviço](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Detalhes%20do%20Servi%C3%A7o.PNG)

Permissões opcionais
![Permissões](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Permiss%C3%B5es%20Opcionais.PNG)

Concluir primeira parte
![Concluir](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Concluir%20P1.PNG)

Clicar no lápis na conta criada para editar:
![Editar](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Editar%20contas%20de%20servi%C3%A7o.PNG)

Clicar em CHAVES e ADICIONAR CHAVE
![Adicionar chave](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Chaves.PNG)

Clicar em JSON e depois CRIAR
![Criar JSON](https://github.com/pycriador/pyJumpCloud/blob/b78b4fcdd44867c3ab579fcb984cc44723cb635e/imagens/Criar%20chave%20JSON.PNG)

#### Documentações úteis:

* [JumpCloud API](https://docs.jumpcloud.com/api/2.0/index.html#operation/bulk_usersCreate)
* [Google QuickStart Python](https://developers.google.com/sheets/api/quickstart/python)
* [OAuth 2.0 Server to Server](https://developers.google.com/identity/protocols/oauth2/service-account)
