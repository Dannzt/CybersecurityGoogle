
<details>	
 <summary><b> Networl </b> </b></summary> 
 
week 5
--------
O tópico desta semana é a troca básica de chaves: como configurar uma chave secreta entre duas partes. Por enquanto, consideramos apenas protocolos seguros contra espionagem. Essa pergunta motiva os principais conceitos de criptografia de chave pública, mas antes de criarmos sistemas de chave pública, precisamos fazer um breve desvio e abordar alguns conceitos básicos da teoria dos números computacionais. Começaremos com algoritmos que remontam à antiguidade (Euclides) e chegaremos até Fermat, Euler e Legendre. Também mencionaremos de passagem alguns conceitos úteis da matemática do século XX. Na próxima semana, faremos bom uso do nosso trabalho árduo desta semana e construiremos vários sistemas de criptografia de chave pública.


Modulo 3:

Com o avanço da tecnologia, a segurança cibernética fica cada vez mais evidente, com isso a CIA (**tríade Confiança, integridade e disponibilidade) é um modelo de segurança , com a cia e a instalação de frameworks diminuímos ricos e vulnerabilidades** 

Network

Os CSPs oferecem três categorias principais de serviços:

- **Software como serviço (SaaS)** refere-se a conjuntos de software operados pelo CSP que uma empresa pode usar remotamente sem hospedar o software.
- **Infraestrutura como serviço** **(IaaS)** refere-se ao uso de componentes de computador virtuais oferecidos pelo CSP. Eles incluem contenções virtuais e armazenamento que são configurados remotamente por meio da API ou do console da Web do CSP. Os serviços de computação e armazenamento em nuvem podem ser usados para operar aplicativos existentes e outras cargas de trabalho de tecnologia sem modificações significativas. Os aplicativos existentes podem ser modificados para aproveitar os recursos de disponibilidade, desempenho e segurança que são exclusivos dos serviços do provedor de nuvem.
- **Plataforma como serviço (PaaS)** refere-se a ferramentas que os desenvolvedores de aplicativos podem usar para projetar aplicativos personalizados para sua empresa. Os aplicativos personalizados são projetados e acessados na Nuvem e usados para as necessidades comerciais específicas de uma empresa.

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c39ccecf-d934-4a0a-b0a2-49b90fe32511/a24561a7-0094-43b2-8cfd-cff70ff69438/image.png)

## O modelo TCP/IP

O **modelo TCP/IP** é uma estrutura usada para visualizar como os dados são organizados e transmitidos em uma rede. Esse modelo ajuda os engenheiros de rede e os analistas de segurança de rede a conceituar os processos na rede e a comunicar onde ocorrem interrupções ou ameaças à segurança.

O modelo TCP/IP tem quatro camadas: a camada de acesso à rede, a camada de Internet, a camada de transporte e a camada do aplicativo. Ao solucionar problemas na rede, os profissionais de segurança podem analisar quais camadas foram afetadas por um ataque com base nos processos envolvidos em um incidente.

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c39ccecf-d934-4a0a-b0a2-49b90fe32511/378a7396-8560-4b12-9847-a8795f7eec73/image.png)

Camada de acesso à rede: a famosa camada de enlace de dados,  é a camada que faz a criação de pacotes de dados e sua transição para a rede.

O protocolo de resolução de endereço (ARP) faz parte dessa camada.

A camada de rede é responsável por receber os pacotes de dados e passar 

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c39ccecf-d934-4a0a-b0a2-49b90fe32511/3a34803c-9c47-44c1-ba8b-93987fc97aee/image.png)

## Camada 7: camada do aplicativo

A camada do aplicativo inclui os processos que envolvem diretamente o usuário comum. Essa camada inclui todos os protocolos de rede que os aplicativos de software usam para conectar um usuário à Internet. Essa característica é a que identifica a camada do aplicativo: a conexão do usuário à Internet por meio de aplicativos e solicitações.

Um exemplo de um tipo de comunicação que ocorre na camada do aplicativo é o uso de um navegador da Web. O navegador da Internet usa HTTP ou HTTPS para enviar e receber informações do servidor do site. O aplicativo de e-mail usa o protocolo de transferência de correio simples (SMTP) para enviar e receber informações de e-mail. Além disso, os navegadores da Web usam o protocolo DNS (sistema de nomes de domínio) para traduzir os nomes de domínio do site em endereços IP que identificam o servidor da Web que hospeda as informações do site.

## Camada 6: camada de apresentação

As funções da camada de apresentação envolvem a tradução de dados e a criptografia para a rede. Essa camada adiciona e substitui dados por formatos que podem ser compreendidos pelos aplicativos (camada 7) nos sistemas de envio e recebimento. Os formatos na extremidade do usuário podem ser diferentes daqueles do sistema receptor. Os processamentos na camada de apresentação exigem o uso de um formato padronizado.

Algumas funções de formatação que ocorrem na camada 6 incluem criptografia, compactação e confirmação de que o conjunto de códigos de caracteres pode ser interpretado no sistema receptor. Um exemplo de criptografia que ocorre nessa camada é o SSL, que criptografa os dados entre os servidores da Web e os navegadores como parte de sites com HTTPS.

## Camada 5: camada de sessão

Uma sessão descreve quando uma conexão é estabelecida entre dois dispositivos. Uma sessão aberta permite que os dispositivos se comuniquem entre si. Os protocolos da camada de sessão mantêm a sessão aberta enquanto os dados estão sendo transferidos e encerram a sessão quando a transmissão é concluída.

A camada de sessão também é responsável por atividades como autenticação, reconexão e definição de pontos de verificação durante uma transferência de dados. Se uma sessão for interrompida, os pontos de verificação garantem que a transmissão seja retomada no último ponto de verificação da sessão quando a conexão for retomada. As sessões incluem uma solicitação e uma resposta entre aplicativos. As funções na camada de sessão respondem a solicitações de serviço de processos na camada de apresentação (camada 6) e enviam solicitações de serviços para a camada de transporte (camada 4).

## Camada 4: camada de transporte

A camada de transporte é responsável pela entrega de dados entre dispositivos. Essa camada também lida com a velocidade da transferência de dados, com o Fluxo da transferência e com a divisão dos dados em segmentos menores para facilitar o transporte. Segmentação é o processo de dividir uma grande transmissão de dados em partes menores que podem ser processadas pelo sistema receptor. Esses segmentos precisam ser remontados em seu destino para que possam ser processados na camada de sessão (camada 5). A velocidade e a taxa da transmissão também precisam corresponder à velocidade da conexão do sistema de destino. O TCP e o UDP são protocolos da camada de transporte.

## Camada 3: camada de rede

A camada de rede supervisiona o recebimento dos frames da camada de enlace de dados (camada 2) e os entrega ao destino pretendido. O destino pretendido pode ser encontrado com base no endereço que reside no frame dos pacotes de dados. Os pacotes de dados permitem a comunicação entre duas redes de computadores. Esses pacotes incluem endereços IP que informam aos roteadores para onde devem ser enviados. Eles são roteados da rede de envio para a rede de recebimento.

## Camada 2: camada de enlace de dados

A camada de enlace de dados organiza o envio e o recebimento de pacotes de dados em uma única rede. A camada de enlace de dados abriga as trocas de rede locais e as placas de interface de rede (NIC) nos dispositivos locais.

Protocolos como o protocolo de controle de rede (NCP), o controle de link de dados de alto nível (HDLC) e o protocolo de controle de link de dados síncrono (SDLC) são usados na camada de enlace de dados.

## Camada 1: camada física

AS como o nome sugere, a camada física corresponde ao hardware físico envolvido na transmissão da rede. Hubs, modems a cabo e os cabos e a fiação que os conectam são considerados parte da camada física. Para trafegar por um cabo Ethernet ou coaxial, um pacote de dados precisa ser traduzido em um fluxo de 0s e 1s. O fluxo de 0s e 1s é enviado através da fiação e dos cabos físicos, recebido e, em seguida, passado para níveis mais altos do modelo OSI.

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/c39ccecf-d934-4a0a-b0a2-49b90fe32511/22556229-2d20-4ed0-9b48-f846945f6fba/image.png)

### **Wi-Fi Protected Access**

O Wi-Fi Protected Access (WPA) foi desenvolvido em 2003 para aprimorar o WEP, resolver os problemas de segurança que ele apresentava e substituí-lo. O WPA sempre foi planejado para ser uma medida de transição, de modo que a compatibilidade com versões anteriores pudesse ser estabelecida com hardware mais antigo.

As falhas do WEP estavam no próprio protocolo e em como a criptografia era usada. O WPA abordou esse ponto fraco usando um protocolo chamado TKIP (Temporal Key Integrity Protocol). O algoritmo de criptografia WPA usa chaves secretas maiores que as do WEP, o que torna mais difícil adivinhar a chave por tentativa e erro.

O WPA também inclui uma verificação de integridade da mensagem que inclui uma tag de autenticação de mensagem em cada transmissão. Se um agente mal-intencionado tentar alterar a transmissão de alguma forma ou reenviá-la em outro momento, a verificação de integridade da mensagem do WPA identificará o ataque e rejeitará a transmissão.

Apesar dos aprimoramentos de segurança do WPA, ele ainda tem vulnerabilidades. Agentes mal-intencionados podem usar um ataque de reinstalação de chave (ou ataque KRACK) para descriptografar transmissões usando o WPA. Os atacantes podem se inserir no processamento do handshake de autenticação do WPA e inserir uma nova chave de criptografia em vez da chave dinâmica atribuída pelo WPA. Se eles definirem a nova chave com todos os zeros, é como se a transmissão não fosse criptografada.

Devido a essa vulnerabilidade significativa, o WPA foi substituído por uma versão atualizada do protocolo chamada WPA2.

### **WPA2 E WPA3**

### **WPA2**

A segunda versão do Wi-Fi Protected Access, conhecida como WPA2, foi lançada em 2004. O WPA2 aprimora o WPA usando o Padrão de Criptografia Avançada (AES). O WPA2 também aprimora o uso do TKIP pelo WPA. O WPA2 usa o protocolo CCMP (Counter Mode Cifra de bloco encadeada para autenticação de mensagens), que fornece encapsulamento e garante a autenticação e a integridade das mensagens. Devido à força do WPA2, ele é considerado o padrão de segurança para todas as transmissões Wi-Fi atuais. O WPA2, como seu antecessor, é vulnerável a ataques KRACK. Isso levou ao desenvolvimento do WPA3 em 2018.

### **Personalização**

O modo pessoal do WPA2 é mais adequado para redes de computadores domésticas por vários motivos. É fácil de implementar e a configuração inicial leva menos tempo para a versão pessoal do que para a versão corporativa. A frase secreta global da versão pessoal do WPA2 precisa ser aplicada a cada computador e ponto de acesso (PA) em uma rede. Isso a torna ideal para redes de computadores domésticas, mas impossível de gerenciar em organizações.

### **Empresarial**

O modo WPA2 Enterprise funciona melhor para aplicativos comerciais. Ele fornece a segurança necessária para redes sem fio em ambientes comerciais. A configuração inicial é mais complicada que a do modo pessoal WPA2, mas o modo enterprise oferece controle individualizado e centralizado sobre o acesso Wi-Fi a uma rede de computadores. Isso significa que os administradores de rede podem conceder ou remover o acesso de usuários a uma rede a qualquer momento. Os usuários nunca têm acesso às chaves de criptografia, o que impede que possíveis atacantes recuperem as chaves de rede de computadores individuais.

### **WPA3**

O WPA3 é um protocolo Wi-Fi seguro e está crescendo em uso à medida que mais dispositivos compatíveis com o WPA3 são lançados. Estas são as principais diferenças entre o WPA2 e o WPA3:

- O WPA3 aborda a vulnerabilidade do handshake de autenticação para ataques KRACK, que é apresentada no WPA2.
- O WPA3 usa Simultaneous Authentication of Equals (SAE), um acordo de compartilhamento de chave de cifra autenticado por senha. Isso impede que os atacantes baixem os dados das conexões de rede sem fio para seus sistemas e tentem decodificá-los.
- O WPA3 aumentou a criptografia para tornar as senhas mais seguras, usando criptografia de 128 bits, com o modo WPA3-Enterprise oferecendo criptografia opcional de 192 bits.

## Acesso remoto e VPNs site a site

Os usuários individuais usam VPNs de acesso remoto para estabelecer uma conexão entre um dispositivo pessoal e um servidor VPN. As VPNs de acesso remoto criptografam os dados enviados ou recebidos por meio de um dispositivo pessoal. A conexão entre o usuário e a VPN de acesso remoto é estabelecida pela Internet.

As empresas usam VPNs site a site principalmente para estender sua rede a outras redes e locais. Isso é particularmente útil para organizações que têm muitos escritórios em todo o mundo. O IPsec é comumente usado em VPNs site a site para criar um túnel criptografado entre a rede principal e a rede remota. Uma desvantagem das VPNs site a site é a complexidade de configuração e gerenciamento em comparação com as VPNs remotas.

## VPN WireGuard vs. VPN IPsec

O WireGuard e o IPSec são dois protocolos de VPN diferentes usados para criptografar o tráfego em um túnel de rede seguro. A maioria dos provedores de VPN oferece uma variedade de opções de protocolos de VPN, como WireGuard ou IPsec. Em última análise, a escolha entre IPSec e WireGuard depende de muitos fatores, incluindo velocidades de conexão, Compatibilidade com a Infraestrutura de rede existente e necessidades comerciais ou individuais.

### VPN WireGuard

O WireGuard é um protocolo VPN de alta velocidade, com criptografia avançada, para proteger os usuários quando estiverem acessando a Internet. Ele foi projetado para ser simples de configurar e manter. O WireGuard pode ser usado tanto para conexão site a site quanto para conexões cliente-servidor. O WireGuard é relativamente mais novo que o IPsec e é usado por muitas pessoas devido ao fato de que sua velocidade de download é aprimorada pelo uso de menos linhas de código. O WireGuard também é um código aberto, o que facilita a implantação e a depuração pelos usuários. Esse protocolo é útil para processos que exigem velocidades de download mais rápidas, como streaming de conteúdo de vídeo ou download de arquivos grandes.

### VPN IPSec

O IPSec é outro protocolo de VPN que pode ser usado para configurar VPNs. A maioria dos provedores de VPN usa o IPSec para criptografar e autenticar pacotes de dados a fim de estabelecer conexões seguras e criptografadas. Como o IPSec é um dos primeiros protocolos de VPN, muitos sistemas operacionais suportam o IPSec dos provedores de VPN.

Embora o IPSec e o WireGuard sejam ambos protocolos VPN, o IPSec é mais antigo e mais complexo que o WireGuard. Alguns clientes podem preferir o IPSec devido ao seu histórico de uso mais longo, testes de segurança extensivos e adoção generalizada. Entretanto, outros podem preferir o WireGuard devido ao seu potencial de melhor desempenho e configuração mais simples.

### DoS (Denial of service attack)

Um ataque DoS é uma enxurrada de informações no server que derruba o servidor.

### DDoS (Distributed denial of service attack)

é um ataque DoS em conjunto com DIVERSOS COMPUTADORES OU SERVIDORES em lugares distintos. 

Pode ser um pacote de informações complexas que deixam os roteadores demorando pra processar a quantidades de dados.

alguns exemplos de ataques DoS:

- **SYN attack (synchronize flood attack**: um ataque com uma inundação de pacotes syn… eles utilizam as politicas de handshack do modelo TCP protocol que manda uma quantidade absurda de syn para o serv pegar, encaminhar pro computador, voltar pro serv e autentificar no seu pc, como é um movimento muito complexo utilizam para derrubarem servidores ou sobrecarregar.

- ICMP flood attack : o ICMP é o protocolo de envio de mensagens, caso você mande uma mensagem e a mensagem vir errada… existe um erro de comunicação com o serv. (ou problemas de cripto como vi no curso)
    
    O DoS utilizando ICMP funciona funciona quase da mesma forma do SYN, ele envia varias mensagens repetidas vezes em questões de segundos, fazendo com que a banda larga comece a só controlar essa sequencia de mensagens. 
    
    Ambas os ataques são sobre grandes números de solicitações e sobrecarregam o server.
    
- Ping of death: ao contrario dos outros casos, utilizando um ping maior que o server consegue aguentar, no caso o ICMP, pingando o server com um tamanho maiores que 64 KB. e sobrecarregando o servidor.

## **tcpdump**

**o tcpdump** é um analisador de protocolo de rede de linha de comando. Ele é popular, leve - o que significa que usa pouca memória e tem baixo uso da memória - e usa a biblioteca libpcap de código aberto. O tcpdump é baseado em texto, o que significa que todos os comandos do tcpdump são executados no terminal. Ele também pode ser instalado em outros sistemas operacionais baseados em Unix, como o macOS®. Ele vem pré-instalado em muitas distribuições Linux.

o tcpdump fornece uma breve análise de pacotes e converte as principais informações sobre o Tráfego de rede em formatos facilmente lidos por humanos. Ele imprime informações sobre cada pacote diretamente em seu terminal. O tcpdump também exibe o endereço IP de origem, os endereços IP de destino e os números de porta que estão sendo usados nas comunicações.

## Interpretação da saída

o tcpdump imprime a saída do comando como interceptação de pacotes na linha de comando e, opcionalmente, em um arquivo de log, depois que um comando é executado. A saída de uma captura de pacote contém muitas informações importantes sobre o Tráfego de rede.

!https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/B-PaECh0ToSFgBWpFczYZg_4896abe8c06443f08eec4dc003dcf8f1_image.png?expiry=1732492800000&hmac=pPZ8kq7YnYPGXNoUuP2_wbny9RuE4mlRoGDAnnxLWbI

Algumas informações que você recebe de uma captura de pacote incluem:

- **Timestamp**: A saída começa com o registro de data e hora, formatado como horas, minutos, segundos e frações de segundo.
- **Source IP:** a origem do pacote é fornecida por seu endereço IP de origem.
- **Source port**: Esse número de porta é o local de origem do pacote.
- **Destination IP**: o endereço IP de destino é o local para onde o pacote está sendo transmitido.
- **Destination port**: Esse número de porta é o local para onde o pacote está sendo transmitido.

## Usos comuns

o tcpdump e outros analisadores de protocolo de rede são comumente usados para capturar e visualizar comunicações de rede e para coletar estatísticas sobre a rede, como na solução de problemas de desempenho da rede. Eles também podem ser usados para:

- Estabelecer uma Linha de Base para padrões de tráfego de rede e Métricas de utilização de rede.
- Detectar e identificar tráfego malicioso
- Criar alertas personalizados para enviar as notificações certas quando surgirem problemas de rede ou ameaças à segurança.
- Localizar mensagens instantâneas (IM), tráfego ou pontos de acesso sem fio não autorizados.

No entanto, os atacantes também podem usar os analisadores de protocolo de rede de forma maliciosa para obter informações sobre uma rede específica. Por exemplo, os atacantes podem capturar pacotes de dados que contenham informações confidenciais, como nomes de usuário e senhas de contas. AS como analista de segurança cibernética, é importante entender a finalidade e os usos dos analisadores de protocolo de rede.
--------
 
-----------------------------------------------------------------------------------------------------------------------------------------------
  </details>
No entanto, os atacantes também podem usar os analisadores de protocolo de rede de forma maliciosa para obter informações sobre uma rede específica. Por exemplo, os atacantes podem capturar pacotes de dados que contenham informações confidenciais, como nomes de usuário e senhas de contas. AS como analista de segurança cibernética, é importante entender a finalidade e os usos dos analisadores de protocolo de rede.
