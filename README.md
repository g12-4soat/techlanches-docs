<p dir="auto"><img src="https://github.com/g12-4soat/tech-lanches/blob/main/src/TechLanches/Adapter/Driver/TechLanches.Adapter.API/wwwroot/SwaggerUI/images/android-chrome-192x192.png" alt="TECHLANCHES" title="TECHLANCHES" align="right" height="60" style="max-width: 100%;"></p>

# Tech Lanches Docs
Projeto Tech Challenge Fase 4

Repositório dedicado às documentações do TechChallenge da FIAP - Turma 4SOAT.

# Descrição

Este projeto faz parte do curso de pós-graduação em Arquitetura de Software oferecido pela FIAP. O objetivo é armazenar todas documentações referentes à aplicação Tech Lanches e justificar escolhas arquiteturais.

# Arquitetura microserviços

<p dir="auto"><img src="https://github.com/g12-4soat/techlanches-docs/blob/feature/readme/docs/fase5/TechLanchesArchitecture-aws-micro-service.png" alt="TECHLANCHES" title="TECHLANCHES" style="max-width: 100%;"></p>

# Diagrama Saga Coreografada

<p dir="auto"><img src="https://github.com/g12-4soat/techlanches-docs/blob/feature/readme/docs/fase5/TechLanchesArchitecture-saga-coreografada.png" alt="TECHLANCHES" title="TECHLANCHES" style="max-width: 100%;"></p>

# Justificativa Uso Saga Coreografada

Optamos pelo padrão de Saga coreografada em nosso sistema de microserviços pelos seguintes motivos:

1. **Simplicidade e Menor Sobrecarga de Gerenciamento**: Com poucos serviços e uma equipe única de manutenção, a coreografia é mais simples de implementar e gerenciar.
   
2. **Descentralização e Independência dos Serviços**: Cada serviço reage a eventos de forma autônoma, facilitando o desenvolvimento, a implantação e a escalabilidade independentes.

3. **Redução de Acoplamento**: A comunicação por eventos promove um baixo acoplamento entre serviços, permitindo modificações e evoluções sem impactos significativos em outros componentes.

4. **Escalabilidade e Resiliência**: A ausência de um orquestrador central elimina pontos únicos de falha e melhora a capacidade de resposta sob alta carga.

5. **Ajuste ao Tamanho e Complexidade do Projeto**: Para nosso contexto, com um número limitado de serviços, a coreografia evita a sobrecarga de um orquestrador central, proporcionando uma solução proporcionalmente adequada.
