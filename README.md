# LiterAlura — estrutura inicial

Estrutura inicial Spring Boot com JPA e driver PostgreSQL. O código disponível contém a inicialização da aplicação; ainda não implementa catálogo, pesquisas ou integração com API de livros.

## Tecnologias

- Java 17
- Spring Boot 4
- Maven
- Spring Data JPA
- PostgreSQL

## Funcionalidades e utilização

Configure um PostgreSQL local e as propriedades de conexão antes de iniciar. O teste de contexto também depende do banco.

## Como executar

```bash
git clone https://github.com/EuGeanCarlos/LiterAlura.git
cd LiterAlura
mvn test
mvn spring-boot:run
```

Requer JDK compatível com pom.xml e Maven 3.9+. Testes Spring podem exigir banco/serviços locais configurados.

## Demonstração e publicação

Execução local. Nenhuma demonstração nova foi confirmada nesta etapa.

GitHub Pages hospeda arquivos estáticos e não executa Java, Node.js, PHP ou Python. As dependências de servidor deste projeto devem ser executadas em ambiente apropriado.

## Estrutura versionada

```text
.gitattributes
.gitignore
.mvn/wrapper/maven-wrapper.properties
mvnw
mvnw.cmd
pom.xml
src/main/java/br/com/literalura/literalura/LiteraluraApplication.java
src/main/resources/application.properties
src/test/java/br/com/literalura/literalura/LiteraluraApplicationTests.java
```

## Status

Protótipo / projeto de estudo em desenvolvimento. A descrição acima distingue o que está implementado das dependências ou etapas pendentes.

## Autor e créditos

**Gean Carlos** — estudante de Engenharia de Computação, UEMA.

[GitHub](https://github.com/EuGeanCarlos)

Licenças, autoria compartilhada e atribuições existentes no código e nos materiais originais permanecem aplicáveis.

## Validação desta auditoria — 14/10/2026

Sem publicação nova confirmada. mvn test falhou no carregamento do contexto: não há datasource URL configurada e não há banco embarcado. Configurar PostgreSQL para testar o esqueleto existente.
