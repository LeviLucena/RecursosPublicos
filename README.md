# Monitoramento de Recursos Públicos - Estado de São Paulo

Este projeto fornece uma plataforma interativa para monitoramento e análise dos recursos públicos do Estado de São Paulo. Utilizando gráficos e visualizações dinâmicas, ele permite que os usuários acompanhem o orçamento, gastos por setor, arrecadação de impostos, investimentos em educação, dívida pública e investimentos em inovação e tecnologia.

![image](https://github.com/user-attachments/assets/a07db1ce-c963-42be-b581-ecb20dfd1ef6)


## Dados Fictícios e Integração com Dados Reais

🔍 **Dados Fictícios:** Os dados apresentados neste projeto são fictícios e foram criados para fins de demonstração e visualização. Eles servem para ilustrar como o sistema funciona e como os gráficos e análises são apresentados.

🌐 **Integração com Dados Reais:** O projeto foi desenvolvido com a flexibilidade necessária para ser integrado com dados reais. Para utilizar dados reais, você pode integrar o sistema com uma API que forneça informações atualizadas sobre orçamento, gastos, arrecadação, investimentos e dívida pública.

### Como Integrar Dados Reais

1. **Identifique uma API de Dados Públicos:** Busque por APIs que disponibilizem dados financeiros e orçamentários do governo do Estado de São Paulo ou de outras fontes confiáveis.

2. **Configure a Conexão com a API:** Utilize JavaScript para fazer requisições HTTP (usando `fetch`, `axios` ou outra biblioteca) para a API e obter os dados em formato JSON.

3. **Atualize os Dados no Sistema:** Substitua os dados fictícios no script com os dados obtidos da API. Ajuste o formato dos dados para que correspondam à estrutura esperada pelo sistema.

4. **Atualize as Visualizações:** Garanta que os gráficos e análises sejam atualizados com os dados reais. Ajuste a função `updateCharts` para processar e exibir as informações provenientes da API.

5. **Testes e Validação:** Teste o sistema com os dados reais para garantir que todas as visualizações e análises estejam corretas e funcionando conforme o esperado.

### Exemplo de Integração

Aqui está um exemplo básico de como você poderia substituir os dados fictícios por dados obtidos de uma API:

```javascript
async function fetchRealData() {
    const response = await fetch('URL_DA_API');
    const data = await response.json();

    // Exemplo de como os dados podem ser estruturados
    fullData = {
        years: data.years,
        budget: data.budget,
        education: data.education,
        debt: data.debt,
        innovation: data.innovation,
        sectorSpending: data.sectorSpending,
        taxCollection: data.taxCollection
    };

    updateCharts();
}

window.onload = function () {
    fetchRealData();
};
```

A integração com dados reais permitirá que o projeto ofereça informações atualizadas e relevantes, melhorando sua utilidade para análise e tomada de decisões.

## Recursos
- 📊 Orçamento Anual: Visualize a evolução do orçamento estadual ao longo dos anos.
- 💸 Gastos por Setor: Analise os gastos distribuídos entre diferentes setores, como saúde, educação, segurança, infraestrutura e outros.
- 💰 Arrecadação de Impostos: Acompanhe a arrecadação de impostos, incluindo ICMS, IPVA, ITCMD e outros.
- 📚 Investimentos em Educação: Monitore os investimentos feitos na área da educação.
- 📉 Evolução da Dívida Pública: Observe a variação da dívida pública ao longo dos anos.
- 🚀 Investimentos em Inovação e Tecnologia: Veja o crescimento dos investimentos em inovação e tecnologia.
Funcionalidades
- 📅 Filtragem por Data: Selecione um intervalo de datas para atualizar as visualizações e análises com base no período escolhido.
- 📈 Gráficos Interativos: Utiliza gráficos interativos para uma visualização clara e detalhada dos dados.
- 📊 Análise Automatizada: Gera análises automatizadas baseadas nos dados exibidos, fornecendo insights relevantes sobre o desempenho financeiro e investimentos.

## Tecnologias Utilizadas
- HTML5 para estruturação do conteúdo da página.
- CSS3 para estilização e layout responsivo.
- JavaScript para funcionalidades interativas e manipulação dos dados.
- Chart.js para geração de gráficos e visualizações de dados.

## Como Usar
1. Selecione o Intervalo de Datas: Utilize o seletor de datas para definir o período que deseja analisar.
2. Atualize os Gráficos: Clique no botão "Atualizar Gráficos" para refletir as mudanças na visualização e nas análises.
3. Explore os Gráficos: Navegue pelos diferentes painéis para visualizar as informações detalhadas sobre orçamento, gastos, impostos, investimentos e dívida.

## Exemplo de Uso
Ao selecionar um intervalo de datas de 2013 a 2050 e clicar em "Atualizar Gráficos", os gráficos serão atualizados para refletir os dados desse período. As análises associadas a cada gráfico também serão ajustadas para fornecer uma visão mais clara do desempenho e das mudanças ao longo dos anos.

## Contribuições
Se você deseja contribuir para este projeto, sinta-se à vontade para enviar pull requests, reportar bugs ou sugerir melhorias. Sua colaboração é bem-vinda!

## Licença
Este projeto é licenciado sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.
