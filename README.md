# Chat-Bot 






<center>
  
  ## Criar ações
  
  ###### Para criar ações ou resposta basta ir no arquivo /config/data.py e adicionar na lista "PhRaseActions", segue o corpo dela.

 ```
  {
    "UUID": 4, 
    "Words": [""], 
    "Actions": {"url": "", "vetores": []},
    "type": "str",
    "payload": [], 
    "response": [""], 
    "action": Math
  }
 ```

 ###### O campo UUID deixe como o tamanho total da lista subtraindo um, a lista "Words" fica responsável por identificar a frase e redirecionar para a ação ou resposta, então vamos para um exemplo, caso vamos querer que o usuário fale - "Gere um valor entre 5 e 4"; Então vamos adicionar na "Words" as palavras "gere", "valor", "entre", "um";

 ###### Adicionando esses valores na lista "Words", vamos partir para o valor "Actions", com isso deixe o campo "url" vazia e adicione no campo "vetores" o vetor principal que vai pegar os valores, como no exemplo passado, vamos ter que pegar o valor 5 e 4, então a palavra anterior a esses valores é a palavra "entre", com isso, basta adicionar a palavra "entre" no campo "vetores"; Deixe agora o campo "type" como "str", deixe o campo "payload" e "response" vazio e no campo "action", coloque a função que pega recebe os valores "5 e 4" que vai ser pego após o vetor "entre".

 ###### Com isso basta finalizar sua função retirando os valores que não são núméricos e continuar sua ação, após concluir sua função, basta retornar falando com a função speak() e dentro de speak getPhrase(), dentro de "getPhrase()" coloque uma lista de possíveis respostas!
</center>
<hr/>

<center>
  
  ## Criar respostas
  
  ###### Para criar ações ou resposta basta ir no arquivo /config/data.py e adicionar na lista "PhRaseActions", segue o corpo dela.

 ```
  {
    "UUID": 4, 
    "Words": [""], 
    "Actions": {"url": "", "vetores": []},
    "type": "str",
    "payload": [], 
    "response": [""], 
    "action": Math
  }
 ```

 ###### O campo UUID deixe como o tamanho total da lista subtraindo um, a lista "Words" fica responsável por identificar a frase e redirecionar para a ação ou resposta, então vamos para um exemplo, caso vamos querer que o usuário fale - "Quem é seu criador?"; Então vamos adicionar na "Words" as palavras "quem", "criador", "seu";

 ###### Adicionando esses valores na lista "Words", vamos partir para o valor "Actions", com isso deixe o campo "url" e "vetores" vazia. Deixe o campo "type" como "str", campo "payload" vazio "[]", agora no campo "response", deixe as possíveis respostas, agora em "action" deixe como  ```False```.

 ###### Após isso o algoritmo já vai identificar que é uma questão de resposta e automaticamente vai responder com alguma resposta aleatória partindo do vetor "response"!
  
</center>

<hr/>

> Curiosidades
> * Feito em menos de dois dias.
> * Em versões futuras vou integrar com o NodeJS.
> 
<br/>

> Bibliotecas
> * os
> * pyautogui
> * gtts
> * playsound
> * math
> * random
> * time

<br/>
    
 ###### Versão do python utilizada: 3.11
 ###### Versão do repositório: 1.0

