# Criação de Dispositivo IoT no Cisco Packet Tracer

## Visão geral

Neste laboratório, utilizei o **Cisco Packet Tracer** para personalizar um dispositivo IoT, transformando um equipamento genérico (`Thing`) em uma câmera de segurança chamada `Security Camera`.

A atividade envolveu a configuração de uma conexão wireless, a verificação do endereço IPv4, o teste de comunicação com um tablet e a criação de um modelo reutilizável.

O objetivo foi entender como **personalizar, conectar e reutilizar dispositivos inteligentes** em uma rede simulada.

<img width="617" height="407" alt="image" src="https://github.com/user-attachments/assets/00b771aa-baa6-4bf3-968a-023e7e1b3989" />

---

## O que pratiquei

* Personalização de um dispositivo IoT no Cisco Packet Tracer.
* Configuração da identificação e aparência de uma câmera.
* Instalação de um adaptador de rede wireless.
* Verificação do endereçamento IPv4.
* Utilização do `ping` para testar a comunicação.
* Criação de um modelo de dispositivo para reutilização em outros projetos.

---

## Como o laboratório foi desenvolvido

1. **Criação:** adição de um dispositivo genérico `Thing` e alteração do nome para `Security Camera`.
2. **Personalização:** configuração do nome, da aparência e do mapeamento de componentes no `Thing Editor`.
3. **Conexão wireless:** seleção do adaptador de rede e verificação da interface `Wireless0`.
4. **Verificação da rede:** consulta ao endereço IPv4 atribuído à câmera.
5. **Teste de comunicação:** utilização de um tablet para enviar um `ping` ao endereço da câmera.
6. **Criação do modelo:** salvamento da câmera personalizada para utilização em outros cenários.
7. **Consulta ao catálogo:** verificação do dispositivo na categoria `Home` do Packet Tracer.

---

## Configurações dos dispositivos

### 1. Câmera de segurança (Security Camera)

O dispositivo genérico foi personalizado para representar uma câmera de segurança conectada à rede wireless.

| Parâmetro               | Configuração                  |
| ----------------------- | ----------------------------- |
| **Dispositivo inicial** | `Thing`                       |
| **Display Name**        | `Security Camera`             |
| **Component Name**      | `Security Camera`             |
| **Slot Mapping**        | `Digital` — `Slot 1`          |
| **Imagem**              | Ícone personalizado de câmera |
| **Adaptador wireless**  | `PT-IOT-NM-1W-AC`             |
| **Interface de rede**   | `Wireless0`                   |
| **Endereçamento IPv4**  | Dinâmico                      |
| **Sub-rede**            | `192.168.25.0/24`             |

### 2. Tablet de testes

O tablet foi utilizado para verificar a comunicação com a câmera por meio da rede.

| Parâmetro             | Configuração                      |
| --------------------- | --------------------------------- |
| **Dispositivo**       | Tablet                            |
| **Função**            | Testar a comunicação com a câmera |
| **Ferramenta**        | `Desktop > Command Prompt`        |
| **Comando utilizado** | `ping`                            |
| **Destino**           | Endereço IPv4 atribuído à câmera  |

### 3. Modelo reutilizável

Após a personalização, a câmera foi selecionada para ser salva como um dispositivo personalizado no Packet Tracer.

| Parâmetro                   | Configuração                   |
| --------------------------- | ------------------------------ |
| **Ferramenta**              | `Tools > Custom Device Dialog` |
| **Dispositivo**             | `Security Camera`              |
| **Categoria**               | `Home`                         |
| **Ações**                   | `Add` e `Save`                 |
| **Local para reutilização** | `End Devices > Home`           |

---

## Testes e verificações

A atividade incluiu a consulta às configurações de rede da câmera e a utilização do comando `ping` a partir de um tablet.

O teste permite verificar se a câmera responde às mensagens enviadas pela rede, ajudando a identificar possíveis problemas de conectividade.

Também foi prevista a abertura de um novo cenário para localizar o modelo personalizado no catálogo de dispositivos.

**Observação:** o teste de conectividade e a consulta ao catálogo fazem parte do procedimento do laboratório. Como não foram apresentados os resultados individuais dessas verificações, não é possível confirmar seu sucesso apenas pela descrição da atividade.

---

## Onde esse conhecimento pode ser aplicado?

**Cenário fictício: instalação de câmeras em uma pequena loja**

Imagine uma loja que precisa instalar câmeras de segurança na entrada, no estoque e na área de atendimento.

Durante a preparação, a equipe de TI percebe que configurar cada dispositivo separadamente pode consumir tempo e causar diferenças entre as configurações.

Para organizar o trabalho, o profissional de TI cria um modelo de câmera com as características necessárias e utiliza esse padrão como referência para os demais equipamentos.

Antes de colocar os dispositivos em funcionamento, também verifica se estão conectados à rede e se respondem aos testes de comunicação.

**Resultado esperado:** facilitar a preparação dos dispositivos, manter um padrão de configuração e identificar possíveis problemas de conexão.

**O que esse cenário ensina:** modelos reutilizáveis ajudam a organizar o trabalho. Em uma instalação real, também seria necessário configurar senhas seguras, proteger a rede e verificar o funcionamento das câmeras.

---

## Principais aprendizados

Com este laboratório, pude praticar conceitos relacionados à configuração e à organização de dispositivos IoT em uma rede.

* **Personalização de dispositivos:** alteração da identificação e aparência de um equipamento.
* **Conectividade wireless:** utilização de um adaptador para conectar dispositivos à rede.
* **Endereçamento IPv4:** identificação dos equipamentos por meio de endereços de rede.
* **Diagnóstico de conexão:** utilização do `ping` para verificar a comunicação.
* **Padronização:** criação de modelos que podem ser reutilizados em outras simulações.

**O principal aprendizado foi entender como configurar e organizar dispositivos IoT e como a padronização pode facilitar atividades de suporte e administração de redes.**

---

## Entendendo os termos técnicos

| Termo                 | Explicação simples                                                       |
| --------------------- | ------------------------------------------------------------------------ |
| **IoT**               | Dispositivos inteligentes conectados à rede, como câmeras e sensores.    |
| **Wireless**          | Conexão de rede sem a utilização de cabos.                               |
| **Adaptador de rede** | Componente que permite conectar um equipamento à rede.                   |
| **IPv4**              | Tipo de endereço utilizado para identificar dispositivos na rede.        |
| **Ping**              | Comando que verifica se outro dispositivo responde pela rede.            |
| **Sub-rede**          | Conjunto de endereços que pertencem a uma mesma rede.                    |
| **Interface**         | Meio de conexão utilizado por um dispositivo para se comunicar.          |
| **Template**          | Modelo que pode ser salvo e reutilizado sem repetir toda a configuração. |

---

## Sobre o laboratório

Atividade desenvolvida no **Cisco Packet Tracer**, com foco na personalização, conectividade wireless e criação de modelos reutilizáveis de dispositivos IoT.

O projeto faz parte do meu portfólio de estudos em **Redes de Computadores, Suporte de TI e Cybersecurity**.
