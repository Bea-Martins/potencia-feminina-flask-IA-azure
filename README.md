# potencia-feminina-flask-IA-azure
Desafio Individual Womakers Code

**1º Passo:** criar um ambiente virtual [python -m venv venv]<br>
**2º Passo:** ativar o ambiente virtual [./venv/scripts/activate]<br>
**3º Passo:** criar um arquivo **requirements.txt**<br>
**4º Passo:** no terminal executar o comando [code .]<br>
**5º Passo:** adicione os pacotes necessários no arquivo **requirements**: flask, python-dotenv e requests<br>
**6º Passo:** instalação dos arquivos [pip install -r requirements.txt]<br>
**7º Passo:** criar um aplicativo principal **app.py**<br>
**8º Passo:** criar uma pasta chamada **templates**<br>
**9º Passo:** dentro da pasta **templates** crie um arquivo **index.html.**<br>
**10º Passo:** definir runtime do flask [set FLASK_ENV=development]<br>
**11º Passo:** executar o app [flask run]<br>
**12º Passo:** adicionar arquivos sensíveis ao **.gitinore**<br>
**13º Passo:** seguir passo a passo [Azure](https://learn.microsoft.com/pt-br/azure/ai-services/translator/create-translator-resource) para utilização da IA<br>
**14º Passo:** criar o arquivo **.env**<br>
**15º Passo:** adicionar mais recursos no arquivo **app.py**<br>
**16º Passo:** criar novo arquivo dentro de **templates** chamado **results.html**<br>
**17º Passo:** Testar!<br>


**OBS sobre a rota principal POST:**
- Lê o texto que o usuário inseriu e o idioma selecionado no formulário
- Lê as variáveis ambientais que criamos anteriormente no arquivo .env
- Cria o caminho necessário para chamar o serviço de Tradução, que inclui o idioma de destino (o idioma de origem é detectado automaticamente)
- Cria as informações de cabeçalho, que incluem a chave para o serviço de Tradução, o local do serviço e uma ID arbitrária para a tradução
- Cria o corpo da solicitação, que inclui o texto que queremos traduzir
- Chama post em requests para chamar o serviço de Tradução
- Recupera a resposta JSON do servidor, que inclui o texto traduzido
- Recupera o texto traduzido 
- Chama render_template para exibir a página de resposta