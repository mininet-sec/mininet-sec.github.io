O Mininet-Sec é uma plataforma de experimentação de cibersegurança em redes programáveis, que permite rápida prototipagem de cenários de segurança, simulação de ataques e testes de ferramentas de segurança ofensiva de forma isolada. A disponibilidade de componentes específicos de segurança somado à capacidade de programabilidade da rede permitem o desenvolvimento rápido, eficaz e especializado de soluções de segurança.

# Visão Geral

A Figura abaixo apresenta uma visão geral do Mininet-Sec.

![Mininet-Sec big picture](/assets/img/mininet-sec-bigpic.png){:.centered}

As principais características da ferramenta são:
- **Emulação de serviços de rede**: Uma das características do Mininet-Sec é a emulação de aplicações ou serviços de rede comuns nos hosts, que ajuda na composição de cenários de ataque ou defesa para experimentos em cibersegurança. Servidores web, servidores de e-mail (SMTP, POP, IMAP), DNS, LDAP, NTP, dentre outros, são alguns exemplos dos mais de 20 serviços que podem ser facilmente instanciados no Mininet-Sec.
- **Biblioteca de nós**: outro recurso disponível no Mininet-Sec é a instanciação de alguns serviços e ferramentas específicas de segurança. Alguns exemplos incluem a criação de Firewalls (baseado em Netfilter/IPTables), SoftTAPs, Switches P4 e Roteadores.
- **Gerenciamento de topologia**: a visualização da topologia permite verificar a conexão dos componentes, possibilita execução de comandos em equipamentos específicos da topologia, e permite adição/remoção de componentes sobre demanda. 
- **Gerador de tráfego**: O Mininet-Sec inclui duas ferramentas de apoio ao experimentador no que tange a geração de tráfego benigno: [D-ITG](https://sources.debian.org/src/d-itg/) e [TRex](https://trex-tgn.cisco.com).

# Mais informações

 - [Download, Instalação e Execução](./getting-started.html)
 - [Publicações](./publications.html)
 - [Tutoriais e documentações de uso](./technical-guides.html)
 - [Equipe de desenvolvimento](./team.html)
 - [Código-fonte e Licenciamento](./source-code-license.html)

# Suporte

Encontrou um bug ou quer requisitar uma funcionalidade? [Reporte aqui!](https://github.com/mininet-sec/mininet-sec/issues)

To contact our team, send an e-mail to **mininet-sec [AT] googlegroups.com**.
