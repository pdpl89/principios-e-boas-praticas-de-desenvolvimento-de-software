# Twelve-Factor App

O 12-Factor App é um **conjunto de princípios e boas práticas** para desenvolver aplicações modernas, especialmente aplicações web e serviços que serão executados em ambientes distribuídos, como nuvens públicas, containers e plataformas de deploy.

Ele é, principalmente, uma metodologia de desenvolvimento e arquitetura de aplicações. Não é um framework de software, uma biblioteca ou uma tecnologia específica.

A metodologia foi criada por engenheiros da Heroku para orientar o desenvolvimento de aplicações que sejam:

* Portáveis: possam ser executadas em diferentes ambientes.
* Escaláveis: consigam lidar com o aumento da demanda.
* Resilientes operacionalmente: sejam mais fáceis de implantar, monitorar e manter.
* Consistentes: tenham processos previsíveis de desenvolvimento, configuração e execução.

A ideia central é estabelecer princípios que orientem as decisões de arquitetura e desenvolvimento, independentemente da linguagem de programação ou do framework utilizado.

O próprio site oficial define o Twelve-Factor App como uma methodology(metodologia) — e explica que ela pode ser aplicada a diferentes linguagens e combinações de serviços. 

Portanto, se você estiver documentando a arquitetura de um projeto, a definição mais precisa seria:

**O 12-Factor App é uma metodologia composta por doze fatores que orientam o desenvolvimento, a configuração, a implantação e a operação de aplicações modernas, com foco em portabilidade, escalabilidade e consistência entre ambientes.**

## Um Exemplo prático

Imagine uma API desenvolvida com Java e Spring Boot, executada em containers Docker e implantada no Kubernetes.

Seguindo os princípios do 12-Factor App, poderiamos ter algo como:

* Guardar credenciais e URLs de serviços fora do código-fonte.

* Declarar as dependências no Maven ou Gradle.

* Gerar um artefato imutável e promover a mesma versão entre ambientes.

* Não armazenar sessões ou arquivos importantes exclusivamente no disco local do container.

* Enviar logs para uma plataforma centralizada.

* Permitir que novas instâncias da API sejam iniciadas para atender ao aumento da demanda.

Perceba a diferença: Spring Boot, Docker e Kubernetes são tecnologias; o 12-Factor App é a metodologia que ajuda a orientar como utilizá-las na construção e operação da aplicação.

Uma aplicação não precisa usar Kubernetes para seguir esses princípios, nem o uso de Kubernetes garante que ela os siga.

