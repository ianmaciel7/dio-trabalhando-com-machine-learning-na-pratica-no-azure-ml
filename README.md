# dio-trabalhando-com-machine-learning-na-pratica-no-azure-ml

1. **Abertura do ML Automatizado**
   - Iniciei o processo abrindo o ML Automatizado.

2. **Definição do Nome do Experimento**
   - Defini o nome do experimento para identificar o projeto.

3. **Definição do Nome do Trabalho**
   - Também defini um nome para o trabalho para referência futura.

4. **Tipo de Tarefa: Regressão**
   - Escolhi o tipo de tarefa como regressão.

5. **Selecionar Dados: Tipo Tabular**
   - Selecionei os dados com o tipo tabular.

6. **Fonte de Dados: Arquivos da Web**
   - Utilizei a opção de arquivos da web como fonte de dados.
   - URL: [https:aka.ms/bike-rentals](https:aka.ms/bike-rentals)

7. **Configurações Adicionais**
   - A única modificação nas configurações foi mudar o cabeçalho de coluna para 'somente o primeiro arquivo tem cabeçalho'.

8. **Configuração de Tarefa: Coluna Destino**
   - Defini a coluna de destino como 'retals'.

9. **Configuração de Adição**
   - Desmarquei a opção de explicar o melhor modelo e usar todos os modelos suportados.

10. **Experiência de Criar Modelo**
    - Prossegui com a criação do modelo.

11. **Criação do Ponto de Extremidade**
    - Após a criação do modelo, criei o ponto de extremidade com o modelo criado.

12. **Teste do Ponto de Extremidade com JSON**
    - Realizei um teste no ponto de extremidade usando o seguinte JSON:
    ```json
    {
      "input_data": {
        "data": [
          {
            "day": 10,
            "mnth": 5,
            "year": 2023,
            "season": 3,
            "holiday": 1,
            "weekday": 3,
            "workingday": 1,
            "weathersit": 1,
            "temp": 0.25,
            "atemp": 0.28,
            "hum": 0.45,
            "windspeed": 0.18
          }
        ]
      }
    }
    ```
    - O resultado obtido foi [245.13683060056593].
