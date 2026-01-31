# 🌍 Calculadora EcoTransporte Brasil - Emissões de CO₂

<div align="center">

![Status](https://img.shields.io/badge/status-ativo-success?style=for-the-badge)
![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-blue?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Transformando consciência ambiental em ações sustentáveis**

[✨ Demo Online](https://rborgesleal.github.io/calc-EcoTrip/) • [🚀 Funcionalidades](#-funcionalidades) • [🛠️ Tecnologias](#%EF%B8%8F-tecnologias-utilizadas) • [📚 Como Usar](#-como-usar)

</div>

---

## 📋 Descrição
Projeto de calculadora web para estimar a emissão de CO2 em diferentes tipos de viagens (carro, avião, ônibus, trem, etc.).

## 🎯 Objetivo
Conscientizar usuários sobre o impacto ambiental de suas viagens e ajudar na escolha de meios de transporte mais sustentáveis.

## 🛠️ Tecnologias Utilizadas
- **HTML5**: Estrutura da página
- **CSS3**: Estilização e responsividade
- **JavaScript**: Lógica de cálculo e interatividade
- **Leaflet**: Biblioteca de mapas interativos
- **OpenStreetMap**: Base de mapas e dados geográficos
- **Nominatim API**: Geocodificação e autocomplete de localizações
- **OSRM API**: Cálculo de rotas e distâncias reais

## 📁 Estrutura do Projeto
```
calculadora/
├── index.html          # Página principal com mapa interativo
├── css/
│   └── styles.css      # Estilos responsivos e animações
├── js/
│   └── script.js       # Lógica de cálculo, mapa e autocomplete
└── README.md           # Documentação do projeto
```

## 🎨 Características Visuais
- Design moderno com gradientes
- Cards coloridos por nível de emissão:
  - 🟢 **Verde**: Baixa emissão (< 5 kg CO2)
  - 🟠 **Laranja**: Média emissão (5-20 kg CO2)
  - 🔴 **Vermelho**: Alta emissão (> 20 kg CO2)
- Animações suaves e transições
- Interface 100% responsiva
- Mapa interativo em tela cheia

## 📖 Dados de Emissão

### 🔬 Base Científica

Os valores de emissão de CO₂ são baseados em fontes oficiais e dados brasileiros atualizados:

| Transporte | Emissão (g CO₂/km) | Sustentabilidade | Fonte |
|------------|---------------------|------------------|-------|
| 🚴 Bicicleta | **0** | 🌿 Muito Alto | Zero emissões |
| 🔋 Carro Elétrico | **22** | 🌿 Muito Alto | Mix energético BR (hidrelétricidade) |
| 🚆 Trem/Metrô | **35** | 🌿 Alto | Transporte elétrico de massa |
| 🌱 Carro Híbrido | **51** | 🌱 Alto | Motor duplo (elétrico + combustão) |
| 🚌 Ônibus | **75** | 🌱 Médio | Transporte coletivo (diesel) |
| ✈️ Avião | **123** | ⚠️ Baixo | Voos domésticos (classe econômica) |
| 🏍️ Motocicleta | **130** | ⚠️ Médio-Baixo | Motos 150-300cc (gasolina) |
| 🚗 Carro Gasolina | **148** | 🛑 Muito Baixo | Veículo 1.0-1.4L (flex/gasolina) |

**Fontes de Dados:**
- 🌐 IPCC (Intergovernmental Panel on Climate Change)
- 🌍 DEFRA (UK Department for Environment, Food & Rural Affairs) 2024
- 🇧🇷 Ministério do Meio Ambiente (Brasil)
- ⚡ EPE - Empresa de Pesquisa Energética (Balanço Energético Nacional)

*⚠️ Valores por passageiro. Para veículos, a emissão é dividida pelo número de passageiros.*

### 🏛️ Cidades Disponíveis

**15 Principais Cidades Brasileiras:**

São Paulo • Rio de Janeiro • Belo Horizonte • Brasília • Curitiba • Porto Alegre • Salvador • Fortaleza • Recife • Manaus • Belém • Goiânia • Campinas • Santos • Florianópolis

**Mais de 100 rotas pré-cadastradas** com distâncias reais entre cidades.

## 🚀 Como Usar

### 🔧 Pré-requisitos

- Navegador moderno (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Conexão com internet (para CDNs de Chart.js e Leaflet.js)
- JavaScript habilitado

### ⚡ Instalação Local

1. **Clone o repositório**

```bash
git clone https://github.com/rborgesleal/calc-EcoTrip
cd calc-EcoTrip
```

2. **Abra no navegador**

```bash
# Opção 1: Abrir diretamente
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux

# Opção 2: Servidor local simples (recomendado)
python -m http.server 8000
# Acesse: http://localhost:8000
```

**Nota**: Não há necessidade de instalação de dependências, build ou servidor. O projeto roda diretamente no navegador!

### 🎮 Passo a Passo

1. Abra o arquivo `index.html` em seu navegador
2. **Digite o local de origem** no primeiro campo (ex: "São Paulo, SP")
   - Aguarde as sugestões de autocomplete aparecerem
   - Selecione a localização desejada
3. **Digite o destino** no segundo campo (ex: "Rio de Janeiro, RJ")
   - Selecione a localização da lista de sugestões
4. Clique em **"🔍 Buscar Rota"**
   - O mapa mostrará a rota com marcadores de origem e destino
   - A distância e tempo estimado serão calculados automaticamente
5. (Opcional) Ajuste o **número de passageiros** para veículos pessoais
6. Clique em **"Calcular Emissões"**
7. Visualize os resultados **comparativos de todos os meios de transporte**
   - Ordenados do mais sustentável ao menos sustentável
   - Com destaque para a melhor opção ambiental

### 💡 Dicas Avançadas

- **Comparação Rápida**: Calcule o mesmo trajeto com diferentes transportes
- **Análise Mensal**: Use a frequência para projetar impacto anual
- **Exportação**: Baixe seu histórico em JSON para planilhas
- **Mapa Interativo**: Arraste os marcadores para ajustar distâncias
- **Clique nas Cidades**: Selecione origem e destino clicando diretamente no mapa

## 📊 Fatores de Emissão (estimativas médias)
- **🚗 Carro (gasolina)**: ~120g CO2/km
- **🚙 Carro (diesel)**: ~110g CO2/km
- **⚡ Carro (elétrico)**: ~50g CO2/km
- **✈️ Avião (voo curto)**: ~250g CO2/km
- **🛫 Avião (voo longo)**: ~150g CO2/km
- **🚌 Ônibus**: ~50g CO2/km
- **🚆 Trem (elétrico)**: ~14g CO2/km
- **🏍️ Motocicleta**: ~100g CO2/km

*Valores calculados por passageiro para veículos compartilháveis (carros e motos)*

## 🌱 Funcionalidades
- [x] **Mapa interativo** com Leaflet e OpenStreetMap
- [x] **Autocomplete de cidades** para origem e destino
- [x] **Cálculo automático de distância** usando rotas reais (OSRM)
- [x] **Comparação entre todos os meios de transporte**
- [x] **Visualização de rota no mapa** com marcadores e linha de trajeto
- [x] **Tempo estimado de viagem** (modo carro)
- [x] **Cálculo de emissão por passageiro** para veículos compartilháveis
- [x] **Cards coloridos** por nível de emissão (verde/laranja/vermelho)
- [x] **Destaque da melhor opção ambiental**
- [x] **Cálculo de árvores necessárias** para compensação
- [x] **Interface responsiva** para mobile e desktop
- [ ] Visualização gráfica dos resultados (gráfico de barras)
- [ ] Dicas de compensação de carbono
- [ ] Histórico de viagens calculadas
- [ ] Exportação de relatórios em PDF

## 📝 Roteiro de Desenvolvimento

### ✅ Fase 1: Estrutura Básica (Concluída)
1. ✅ Criar HTML com formulário de entrada
2. ✅ Estilizar página com CSS
3. ✅ Implementar cálculos básicos em JavaScript

### ✅ Fase 2: Funcionalidades Avançadas (Concluída)
1. ✅ Integração com mapa interativo (Leaflet)
2. ✅ Implementar autocomplete de localizações
3. ✅ Cálculo de rotas reais com OSRM
4. ✅ Sistema de comparação entre todos os transportes
5. ✅ Validações de formulário

### 🚧 Fase 3: Melhorias (Em Andamento)
1. [ ] Adicionar gráficos e visualizações (Chart.js)
2. [x] Implementar responsividade completa
3. [x] Adicionar animações e transições
4. [ ] Sistema de histórico com localStorage
5. [ ] Exportação de relatórios

## 👨‍💻 Autor
Rodrigo Borges Leal

## 📄 Licença
Projeto educacional - Livre para uso e modificação