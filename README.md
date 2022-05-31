### API de Cotações de Moedas
   API Simples via cURL de Cotações, agora com mais de 150 moedas diferentes!
  
### Conteúdo
   - [Guia de instalação](#installation-guide)
   - [Uso](#uso)
   - [Funções](#funções)
   - [Feedback & Contribuição](#feedback--contribution)

### Guia de instalação
   Instale a classe em seu arquivo
   require_once("CoinsApi.php");

### Uso
  Por exemplo, como chamar a função e conectar-se ao API, o exemplo mostra todas as moedas (descontinuado)

  ```php
     <?php
       require_once("CoinsApi.php");
       $api = new CoinsApi();
       echo $api->all();
  ```

### Funções
  * GET - `last($coin)` {$coin = string USD} -> Retorna moedas selecionadas (atualizado a cada 30 segundos).
  * GET - `daily([])` {[] = Array ["coin" => "USD", "days" => "10"]} -> Retorna o fechamento dos últimos dias.
  * GET - `daily([])` {[] = Array ["coin" => "USD", "start_date" => "20180901", "end_date" => "20180930"]} -> Retorna o fechamento de um período específico
  * GET - `amount([])` {[] = Array ["coin" => "USD", "amount" => "10"]} -> Retorna cotações sequenciais de uma única moeda
  * GET - `amount([])` {[] = Array ["coin" => "USD", "amount" => "10", "start_date" => "20200301", "end_date" => "20200330"]} -> Retorna cotações sequenciais de um período específico
  * GET - `all()` -> Retorna todas as moedas (descontinuado)
  * GET - `format([])`{[] = Array ["coin" => "USD", "format" => "xml"]} -> Formato de resposta

### Códigos das moedas
  * Veja a lista completa de combinações em https://economia.awesomeapi.com.br/xml/available
  * Veja a lista de nomes das moedas https://economia.awesomeapi.com.br/xml/available/uniq

### Moedas com conversão para
  * BRL (Real Brasileiro)
  * USD (Dolar Americano)
  * EUR (Euro)

### Outras conversões
  * USD-BRLT (Dólar Americano para Real Brasileiro Turismo)

### Feedback e contribuição
  * AwesomeAPI
  * Angel Developers
