Monitoramento de Temperatura

Este projeto é um sistema simples de monitoramento de temperatura desenvolvido em Python. Ele simula leituras de sensores de temperatura internas e externas, verifica se os valores estão dentro de faixas aceitáveis e registra os dados em um arquivo de log.

Funcionalidades 🛠️

Simulação de Temperatura: Gera valores aleatórios para sensores interno e externo.

Validação de Intervalos: Verifica se as temperaturas estão dentro das faixas aceitáveis.

Alertas: Emite alertas se alguma temperatura estiver fora do intervalo esperado.

Registro em Arquivo: Salva as leituras em um arquivo chamado temperaturas_log.txt.

Como Executar 🚀

Pré-requisitos:

Python 3 instalado.

Passos:

Clone este repositório:

git clone <URL_DO_REPOSITORIO>

Acesse o diretório do projeto:

cd <NOME_DO_DIRETORIO>

Execute o script:

python monitoramento_temperatura.py

Estrutura do Código 🧩

1. simulate_temperature_sensor()

Simula leituras de temperatura para sensores interno e externo.

Retorna um dicionário com as temperaturas.

2. check_temperature_ranges(temperatures)

Verifica se as leituras estão dentro dos intervalos aceitáveis.

Retorna mensagens de alerta ou indica que os valores estão normais.

3. log_temperatures(temperatures)

Salva as leituras de temperatura em um arquivo de log.

4. Execução Principal (__main__)

Realiza a simulação, verifica os alertas e registra os dados.

Intervalos Aceitáveis 📊

Interna: 20.0°C a 24.0°C.

Externa: 15.0°C a 30.0°C.

Exemplo de Saída 📋

--- Monitoramento de Temperatura ---
Leitura atual - Interna: 21.5°C, Externa: 28.3°C
Todas as temperaturas estão dentro dos intervalos aceitáveis.
Monitoramento concluído.

Melhorias Futuras 🌟

Conectar com sensores reais para monitoramento em tempo real.

Implementar notificações por e-mail para alertas críticos.

Criar uma interface gráfica para exibição dos dados.


Contribuições 🤝

Contribuições são bem-vindas! Para sugerir melhorias ou reportar problemas, abra uma issue ou envie um pull request.

Autor ✒️

[Seu Nome] - Desenvolvedor e Criador do Projeto.
