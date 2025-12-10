# Gest-o-de-Vulnerabilidades
Repositório voltado à fornecer conhecimentos sobre a parte básica dos conhecimentos de Gestão de Vulnerabilidades
# TERMOS SOBRE GESTÃO DE VULNERABILIDADES QUE DEVEM SER CONHECIDOS:

## O QUE É UMA CVE?
Uma **CVE** (Common Vulnerabilities and Explosures), é um catalogo, ou melhor, uma plataforma que guarda as vulnerabilidades e breves informações, como ano, descrição breve, e seu auditor ou onde foi encontrada. 

Criado para se obter de uma forma melhor informações sobre vulnerabilidades e se encontrar de forma mais rapidamente, pois possui a formulação:

```
CVE - AAAA-NNNNN 

AAAA - Refere-se ao ano em que a vulnerabilidade foi reportada.

NNNNN - Obtém-se por uma sequência numérica.
```

Assim, após aprovada torna-se então válida a CVE, tendo então, empresas parceiras pelo mundo todo, com as CVA, empresas parceiras e autorizadas a publicarem requests.

## O que é CVSS?
A CVSS diferente da CVE, não é apenas um catálogo, mas sim uma ordem de descrição das vulnerabilidades. Assim, cria-se uma classificação de 0 a 10, das mais perigosas falhas para exploração.

## Exploit:

O exploit no contexto de cibersegurança nada mais é que a vulnerabilidade explorada, a chave de acesso e como isso é usado como uma ferramenta de intrusão, de acesso, de controle do program. Ele possui nada mais que a falha em si, é o que todo e qualquer hacker procura, ele é a falha, é a chave da porta para ter acesso a uma vulnerabilidade.

## EPSS:
Este termo, Exploit Prediction Scoring System(EPSS) foi criado para nomear e classificar os Exploits, colocando um score (classificação) de 0 a 1 (0% a 100%), fornecendo assim, um indicador de quanto o exploit pode ou não ser explorado. Dessa forma, quanto mais proximo dos 1 maior a probabilidade e facilidade com que a falha seja explorada.

## EPSS X CVSS: QUAL PRIORIZAR?
Para abordarmos isso, primeiramente devemos entender que em casos de que a questão de **severidade teorica de um** contra **atividade e utilização da falha em estado real de atuação**, torna um tanto mais claro.

Dessa maneira, é válido salientar que a maneira mais eficaz de se prevenir é priorizando a correção das falhas em conjunto, visto que, em casos como :

  1- **CVSS ALTO (9.0+) e EPSS (≥8):** Deve-se corrigir imediatamente, pois está sendo utilizada diariamente pelos invasores.

  2- **CVSS Baixo/Médio (Ex.: 5.0) e EPSS Alto (Ex.: >0.7):** **Corrigir Urgentemente.** A falha não parece devastadora (CVSS baixo), mas os atacantes a estão explorando agora! O risco é imediato.

  3- **CVSS Alto (9.0+) e EPSS Baixo (Ex.: <0.05):** **Agendar Correção.** A falha é grave, mas não há evidência de exploração em massa. Ela é importante, mas não a mais urgente.

Assim, conseguimos observar que quanto maior a circunstância dos atacantes estarem aproveitando e utilizando a vulnerabilidade em tempo real, é de uso **URGENTE a correção dessa falha**, ou seja, mesmo que uma falha esteja com um CVSS Alto e não sendo explorada, podemos agendar o seu reparo. Enquanto, se o EPSS estiver alto e o CVSS, baixo, essa tem prioridade, pois está sendo usada no momento da verificação.

## CISA KEV:

Aqui vemos o mais alto grau de exploração, a conclusão final de que o sistema está comprometido, que estão utilizando as informações e que há vulnerabilidade nesse programa. Sendo assim, o **CISA KEV** (Catálogo de Vulnerabilidades Conhecidas e Exploradas) é uma lista mantida pela **CISA** (Cybersecurity and Infrastructure Security Agency), a agência de segurança cibernética do governo federal dos Estados Unidos.

Então para simplificar, o estudo temos essa tabela:
| **Sistema** | **O que ele fornece** | **Como usá-lo** |
| --- | --- | --- |
| **CVE** | O **ID** único da vulnerabilidade (e a descrição). | É a **referência** que você usa para rastrear e discutir a falha. |
| **CVSS** | A **Gravidade** teórica (0.0 a 10.0). | Responde: "Quão ruim *seria* se fosse explorada?" Ajuda a classificar o impacto. |
| **EPSS** | A **Probabilidade** estatística de exploração nos próximos 30 dias (0% a 100%). | Responde: "Quão provável é que a exploração aconteça *em breve*?" Ajuda a otimizar recursos. |
| **CISA KEV** | **Confirmação** de exploração ativa. | Responde: "**A exploração já está acontecendo AGORA**." É a **prioridade absoluta**, independente da pontuação CVSS ou EPSS. |
