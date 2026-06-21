#  Forno Fácil

App mobile para controle de forno elétrico via NFC, com foco em acessibilidade para o público idoso.

>  **Sobre este repositório:** este é um repositório de apresentação (showcase). O código-fonte do projeto é mantido privado, pois o Forno Fácil é um produto com modelo de negócio comercial (B2B, comercializado em conjunto com o equipamento físico). Aqui você encontra a documentação técnica, a arquitetura e a demonstração do projeto.

## Sobre o projeto

O Forno Fácil nasceu para resolver um problema real: a dificuldade que pessoas idosas costumam ter com a tecnologia do dia a dia — nesse caso, controlar um forno elétrico. A solução une um aplicativo mobile simplificado a um forno equipado com NFC, permitindo operar o equipamento com um único toque, sem menus complexos.

## Funcionalidades

- Controle do forno via aproximação NFC, com interface simplificada e acessível
- Firmware ESP32 (Wi-Fi, MQTT, NFC e relé) desenvolvido para o controle físico do equipamento
- Feedback sonoro guiando o usuário em cada etapa (expo-av)
- Animações de orientação durante o uso (Animated API)
- Projeto de hardware documentado: diagramas de fiação e lista de componentes

## Arquitetura

| Camada | Tecnologias |
|---|---|
| Mobile | React Native, Expo, TypeScript |
| Embarcado | ESP32, Wi-Fi, MQTT, NFC, relé |
| Feedback | expo-av, Animated API (React Native) |

> Nota técnica: o fluxo completo do app (onboarding, receitas, preparo, alertas) está implementado, com simulação de leitura NFC e de temperatura no código. O firmware ESP32 já foi desenvolvido; a montagem do protótipo físico e os testes em hardware real são a próxima etapa do projeto.

## Captura de vídeo em formato GIF (sem efeitos sonoros)

<img width="402" height="850" alt="Gif Forno fácil" src="https://github.com/user-attachments/assets/782f38f6-1137-48aa-8935-f1121591c1cb" />

## Capturas de tela

Fluxo completo do app: configuração inicial (feita uma única vez pelo familiar) seguida do uso no dia a dia.

| | | |
|---|---|---|
| ![Splash](01-splash.jpeg) | ![Onboarding](02-onboarding-intro.jpeg) | ![Configurar nome](03-setup-nome.jpeg) |
| Abertura do app | Início da configuração | Passo 1 — nome de quem vai usar |
| ![Conectar NFC](04-setup-nfc.jpeg) | ![Forno conectado](05-setup-sucesso.jpeg) | ![Tela inicial](06-home.jpeg) |
| Passo 2 — conexão com o forno | Passo 3 — configuração concluída | Tela inicial personalizada |
| ![Categoria Carnes](07-categoria-carnes.jpeg) | ![Detalhe da receita](08-receita-detalhe.jpeg) | ![Passo a passo](09-receita-passo-a-passo.jpeg) |
| Lista de receitas por categoria | Detalhe da receita | Passo a passo da receita |
| ![Pré-aquecimento](10-pre-aquecimento.jpeg) | ![Aquecendo](11-aquecendo.jpeg) | ![Forno pronto](12-forno-pronto.jpeg) |
| Aviso de pré-aquecimento | Forno aquecendo, com progresso | Forno pronto, timer iniciado |

## Status do projeto

Em desenvolvimento ativo desde jan/2025.

## Autor

**Luiz Fernando Grimello**
Desenvolvedor Mobile & Full Stack
[GitHub](https://github.com/fernandogrimello) · [LinkedIn](https://www.linkedin.com/in/luiz-fernando-grimello-6568b4358) · fernandogrimello@gmail.com
