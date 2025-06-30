# Base de perguntas
perguntas = [
    {
        "pergunta": "1. O que é um e-mail de phishing?",
        "alternativas": [
            "Um e-mail enviado pelo RH da empresa",
            "Um e-mail com promoções reais de sites confiáveis",
            "Um e-mail falso que tenta enganar o usuário",
            "Um e-mail com newsletter da empresa",
            "Um e-mail de agradecimento de um colega"
        ],
        "resposta": 3
    },
    {
        "pergunta": "2. Qual das opções abaixo é um sinal comum de e-mail de phishing?",
        "alternativas": [
            "Mensagem bem escrita e personalizada",
            "Endereço do remetente confiável",
            "Pedido urgente para clicar em um link",
            "Assinatura da empresa oficial",
            "Anexo em PDF com contrato legítimo"
        ],
        "resposta": 3
    },
    {
        "pergunta": "3. O que você deve fazer ao receber um e-mail suspeito?",
        "alternativas": [
            "Clicar no link para confirmar se é falso",
            "Ignorar e deletar sem relatar",
            "Encaminhar a todos os colegas",
            "Responder pedindo mais informações",
            "Reportar ao setor de TI ou Segurança da Informação"
        ],
        "resposta": 5
    },
    {
        "pergunta": "4. Qual senha é considerada mais segura?",
        "alternativas": [
            "12345678",
            "senha123",
            "meunome2024",
            "Qz$1p!8kL",
            "abcd1234"
        ],
        "resposta": 4
    },
    {
        "pergunta": "5. Qual dessas práticas reduz o risco de phishing?",
        "alternativas": [
            "Acessar links de qualquer e-mail",
            "Utilizar a mesma senha para tudo",
            "Treinamento de conscientização em segurança",
            "Compartilhar senha com colega",
            "Desativar antivírus para abrir anexos"
        ],
        "resposta": 3
    }
]

# Função de pausa
def pausar():
    input('\nPressione ENTER para continuar...')

# Função principal do quiz
def iniciar_quiz():
    pontuacao = 0
    print('\n=== QUIZ SOBRE PHISHING ===\n')
    for q in perguntas:
        while True:
            print(q["pergunta"])
            for i, alt in enumerate(q["alternativas"], start=1):
                print(f'{i} - {alt}')
            resposta = input("Digite o número da resposta correta: ").strip()
            if resposta.isdigit():
                resposta_int = int(resposta)
                if 1 <= resposta_int <= len(q["alternativas"]):
                    if resposta_int == q["resposta"]:
                        print("✅ Resposta correta!\n")
                        pontuacao += 1
                        break
                    else:
                        print("❌ Resposta incorreta! Tente novamente.\n")
                else:
                    print("Número fora do intervalo. Tente novamente.")
            else:
                print("Entrada inválida. Digite um número.")
    print(f"\nQuiz finalizado! Você acertou {pontuacao} de {len(perguntas)} perguntas.")
    pausar()

# Menu principal
def exibir_menu():
    while True:
        print("\n=== MENU DO QUIZ ===")
        print("1 - Iniciar quiz")
        print("0 - Sair")
        opcao = input("Escolha uma opção: ")
        if opcao == '1':
            iniciar_quiz()
        elif opcao == '0':
            print("Saindo...")
            break
        else:
            print("Opção inválida. Tente novamente.")
            pausar()

# Iniciar programa
exibir_menu()
