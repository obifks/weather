import random

def simulate_temperature_sensor():
    """
    Simula leituras de temperatura (em graus Celsius) para um sistema de monitoramento.

    Retorna:
        dict: Leituras simuladas para o sensor interno e externo.
    """
    internal_temp = round(random.uniform(18.0, 25.0), 2)
    external_temp = round(random.uniform(10.0, 35.0), 2)

    return {"Interna": internal_temp, "Externa": external_temp}

def check_temperature_ranges(temperatures):
    """
    Verifica se as temperaturas estão dentro dos intervalos aceitáveis.

    Parâmetros:
        temperatures (dict): Leituras de temperatura.

    Retorna:
        str: Mensagem indicando o status.
    """
    internal = temperatures["Interna"]
    external = temperatures["Externa"]

    alerts = []

    if internal < 20.0 or internal > 24.0:
        alerts.append(f"Alerta: Temperatura interna fora do intervalo: {internal}°C")

    if external < 15.0 or external > 30.0:
        alerts.append(f"Alerta: Temperatura externa fora do intervalo: {external}°C")

    return alerts if alerts else ["Todas as temperaturas estão dentro dos intervalos aceitáveis."]

def log_temperatures(temperatures):
    """
    Salva as leituras de temperatura em um arquivo.

    Parâmetros:
        temperatures (dict): Leituras de temperatura.
    """
    with open("temperaturas_log.txt", "a", encoding="utf-8") as file:
        file.write(f"Interna: {temperatures['Interna']}°C, Externa: {temperatures['Externa']}°C\n")

if __name__ == "__main__":
    print("--- Monitoramento de Temperatura ---")

    # Simular leituras de temperatura
    temperatures = simulate_temperature_sensor()
    print(f"Leitura atual - Interna: {temperatures['Interna']}°C, Externa: {temperatures['Externa']}°C")

    # Verificar alertas
    alerts = check_temperature_ranges(temperatures)
    for alert in alerts:
        print(alert)

    # Registrar leituras
    log_temperatures(temperatures)

    print("Monitoramento concluído.")
