### 1. Introdução

Este projeto explora o uso do **Azure Cognitive Services** para análise de imagens e reconhecimento de texto. O objetivo é demonstrar como os serviços de inteligência artificial da Azure podem ser aplicados para extrair informações de imagens, com exemplos de reconhecimento facial, OCR (reconhecimento óptico de caracteres) e geração de legendas automáticas.

Utilizei os serviços **Face Detection**, **Optical Character Recognition (OCR)** e **Image Analysis** com a funcionalidade de legendas automáticas. Este projeto está estruturado para demonstrar o fluxo de configuração, uso e análise de resultados desses serviços.

### 2. Configuração do Projeto

Para configurar o ambiente, segui os passos abaixo:
1. **Criação de um recurso Azure Cognitive Services**: No [Portal do Azure](https://portal.azure.com), criei uma nova instância do Azure AI Services. Escolhi a região **East US** e utilizei uma assinatura do Azure Subscription 1.
   
2. **Configuração do recurso**: Após criar o serviço, acessei a página do [Vision Studio](https://portal.vision.cognitive.azure.com/), onde fui em "view all resources" e tornei o recurso criado como padrão (default) para facilitar o acesso aos serviços cognitivos.

3. **Testes Práticos**: Utilizei o Vision Studio para praticar cada serviço, verificando a capacidade de detecção facial, extração de texto e descrição de imagens.

### 3. Experimentos Realizados

Para cada teste realizado, armazenei as imagens de entrada na pasta `inputs` e os resultados na pasta `outputs`.

#### Experimento 1: Face Detection
- **Descrição**: Testei o serviço de detecção facial carregando imagens com diferentes números de pessoas e variações (pessoas com e sem máscara).
- **Resultado**: O serviço foi capaz de identificar a presença de rostos, se as pessoas estavam de máscara, e quantas pessoas havia na imagem. O resultado JSON continha detalhes como coordenadas de localização dos rostos.
- **Insight**: Essa funcionalidade pode ser muito útil em sistemas de segurança e controle de presença, fornecendo dados rápidos sobre a situação em uma imagem.

#### Experimento 2: Optical Character Recognition (OCR)
- **Descrição**: Utilizei imagens com textos impressos e manuscritos para avaliar a precisão do OCR na extração de caracteres.
- **Resultado**: O serviço extraiu o texto e apresentou o conteúdo de forma estruturada no JSON, reconhecendo com precisão cada caractere.
- **Insight**: Essa ferramenta é extremamente eficiente para a digitalização de documentos, facilitando a automação de tarefas de entrada de dados em sistemas que necessitam de processamento de documentos.

#### Experimento 3: Image Captions
- **Descrição**: Testei a função de geração de legendas automáticas utilizando uma imagem contendo um diagrama de machine learning.
- **Resultado**: A função criou uma descrição precisa da imagem, como “diagrama mostrando etapas de aprendizado de máquina”, capturando o contexto visual.
- **Insight**: A criação automática de legendas pode ser aplicada em sites para melhorar a acessibilidade e criar metadados automaticamente em bancos de imagens.

### 4. Insights e Aprendizados

Durante o uso dos Azure Cognitive Services, observei a facilidade de configurar e integrar esses serviços em um ambiente. Estes são alguns aprendizados principais:

- **Reconhecimento de imagem e texto**: Esses serviços possuem um potencial significativo para aplicações em segurança, acessibilidade e automação.
- **Facilidade de uso e integração**: A interface do Vision Studio é amigável, permitindo experimentação rápida e entendimento dos resultados.
- **Potencial de expansão**: Futuramente, a integração desses serviços com o Azure Search pode potencializar a criação de sistemas de pesquisa visual e textual mais robustos.

### 5. Próximos Passos

A partir deste projeto inicial, considero realizar as seguintes melhorias e expansões:
- **Integração com banco de dados**: Armazenar os dados extraídos para permitir consultas e análises mais avançadas.
- **Autenticação com reconhecimento facial**: Explorar a possibilidade de utilizar a detecção facial para autenticação em sistemas.
- **Automatização de análise de imagens em larga escala**: Desenvolver um sistema de upload de imagens para análise em tempo real, gerando relatórios automáticos.

### 6. Conclusão

Este projeto demonstrou o poder dos serviços cognitivos da Azure para interpretar informações visuais e textuais, ampliando minhas habilidades técnicas e meu entendimento de aplicações práticas de IA. Esta prática foi enriquecedora, pois não só explorei o potencial da plataforma Azure como aprendi a integrá-la em projetos práticos.

---

### Imagens e prints
Nas pastas Input e Output, inclui prints do portal Azure Vision Studio mostrando o antes e o depois de cada etapa e a funcionalidade do experimento. 

### Links úteis:

- [GitHub - Azure AI Vision: Face](https://github.com/Azure-Samples/azure-ai-vision/tree/main/face)  
- [Documentação Azure - Quickstart com SDK e Identidade](https://learn.microsoft.com/pt-br/azure/ai-services/computer-vision/quickstarts-sdk/identity-client-library?tabs=windows%2Cvisual-studio&pivots=programming-language-csharp)  
- [Microsoft Learning - AI Fundamentals: Face Detection Lab](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html)  
- [Microsoft Learning - AI Fundamentals: OCR Lab](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)  
- [Microsoft Learning - AI Fundamentals: Image Analysis Lab](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html)
  
