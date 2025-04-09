- [voltar](https://github.com/0joseDark/dream-sonho/blob/main/README.md)
- O **ROS (Robot Operating System)** não é um sistema operativo no sentido tradicional, mas sim um conjunto de ferramentas, bibliotecas e convenções para ajudar no desenvolvimento de aplicações robóticas. Ele fornece uma estrutura modular para que diferentes partes de um robô possam comunicar entre si de forma eficiente.

## 🔹 **Principais Conceitos do ROS**
1. **Nó (Node)** 🖥️  
   - Um nó é um processo que executa uma tarefa específica dentro do sistema ROS.
   - Por exemplo, um nó pode controlar os motores, outro pode capturar imagens de uma câmara e outro pode processar sensores.

2. **Tópicos (Topics)** 🔄  
   - São canais de comunicação usados pelos nós para enviar e receber mensagens de forma assíncrona.
   - Exemplo: Um nó de sensores pode publicar leituras num tópico chamado `/sensor_data`, e um nó de controle pode subscrever-se a esse tópico para processar os dados.

3. **Mensagens (Messages)** 📦  
   - Formato de dados usados para a comunicação entre nós.
   - Exemplo: Uma mensagem pode conter a posição de um robô (x, y, θ) ou a intensidade de um sensor.

4. **Serviços (Services)** ⚡  
   - Diferente dos tópicos, que são comunicação contínua, os serviços permitem uma comunicação do tipo pedido e resposta (request-response).
   - Exemplo: Um nó pode enviar um pedido a outro nó para obter a posição atual do robô.

5. **Ações (Actions)** 🎯  
   - Parecido com serviços, mas permitem tarefas demoradas e a obtenção de feedback durante a execução.
   - Exemplo: Um robô pode receber a ordem para se deslocar até um ponto e enviar atualizações durante o percurso.

6. **Pacotes (Packages)** 📦  
   - O código do ROS é organizado em pacotes, que podem conter nós, mensagens, serviços e configurações.
   - Exemplo: Um pacote pode conter o código para controlar um braço robótico.

7. **ROS Master** 🏆  
   - Coordena a comunicação entre os nós.
   - Ele mantém um registo de quais nós existem e quais tópicos estão a ser publicados/subscritos.

## 🔹 **Versões do ROS**
1. **ROS 1 (Clássico)** 🏗️  
   - Usado há muitos anos, mas tem limitações como a falta de suporte nativo para múltiplos robôs em tempo real.
  
2. **ROS 2 (Atual)** 🚀  
   - Mais moderno, suporta melhor robôs distribuídos e comunicação em tempo real.
   - Usa **DDS (Data Distribution Service)** para melhorar a comunicação.

## 🔹 **Como o ROS é Usado?**
- **Robôs móveis** 🤖 (ex.: carros autónomos, drones)
- **Braços robóticos** 🦾 (ex.: produção industrial)
- **Simulação** 🖥️ (ex.: Gazebo, RViz)
- **Visão computacional** 👀 (ex.: OpenCV + ROS)

## 🔹 **Instalação do ROS no Ubuntu**
```bash
sudo apt update
sudo apt install ros-noetic-desktop-full
```
Para ROS 2:
```bash
sudo apt update
sudo apt install ros-humble-desktop
```
