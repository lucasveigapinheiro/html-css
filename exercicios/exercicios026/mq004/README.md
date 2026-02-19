# Media Query Tester 🎯

Uma demonstração interativa de CSS Media Queries que mostra como um site se adapta automaticamente a diferentes dispositivos e tamanhos de tela.

## 📱 Sobre o Projeto

Este é um site educativo que demonstra o conceito de **Media Queries** em CSS. O site detecta automaticamente o tipo de dispositivo e tamanho de tela, adaptando seu visual e conteúdo de acordo.

### 🎨 Funcionalidades

- **Detecção automática de dispositivo**: Celular, tablet, computador, TV e impressão
- **Informações em tempo real**: Largura, altura, orientação e DPI da tela
- **Design responsivo**: Interface que se adapta perfeitamente a qualquer tamanho
- **Animações interativas**: Transições suaves e efeitos visuais atrativos
- **Suporte a impressão**: Layout otimizado para impressão

## 🚀 Como Usar

### Teste Básico
1. Abra o arquivo `index.html` em seu navegador
2. Redimensione a janela do navegador
3. Observe como os ícones e o fundo mudam automaticamente

### Testes Avançados
- **Celular/Tablet**: Use as ferramentas de desenvolvedor (F12) > Toggle Device Toolbar
- **Orientação**: Gire seu dispositivo ou use a ferramenta de orientação
- **Impressão**: Pressione `Ctrl+P` (Windows/Linux) ou `Cmd+P` (Mac) para ver o modo impressão

## 📁 Estrutura do Projeto

```
mq004/
├── index.html              # Página principal
├── estilos/
│   ├── style.css          # Estilos principais e responsivos
│   └── media-query.css    # Media queries específicas
├── js/
│   └── script.js          # JavaScript interativo
└── imagens/               # Ícones dos dispositivos
    ├── icon-phone.png
    ├── icon-tablet.png
    ├── icon-print.png
    ├── icon-pc.png
    └── icon-tv.png
```

## 🎯 Breakpoints Implementados

| Dispositivo | Largura | Background | Status |
|-------------|---------|------------|---------|
| **Celular** | Até 768px | Roxo gradiente | ✅ Ativo |
| **Tablet** | 769px - 1024px | Rosa gradiente | ✅ Ativo |
| **Computador** | 1025px - 1279px | Azul gradiente | ✅ Ativo |
| **TV** | 1280px+ | Verde água gradiente | ✅ Ativo |
| **Impressão** | Print | Branco | ✅ Ativo |

## 🎨 Design System

### Cores Principais
- **Primário**: `#667eea` (Roxo)
- **Secundário**: `#f093fb` (Rosa)
- **Terciário**: `#4facfe` (Azul)
- **Quaternário**: `#a8edea` (Verde água)

### Tipografia
- **Fonte Principal**: 'Segoe UI', sans-serif
- **Ícones**: Font Awesome 6
- **Monospace**: Para valores técnicos

### Componentes
- **Cards**: Bordas arredondadas, sombras suaves
- **Botões**: Gradientes com hover effects
- **Notificações**: Toast messages animados

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **CSS3**: Media queries, gradientes, animações
- **JavaScript**: DOM manipulation, event listeners
- **Font Awesome**: Ícones vetoriais

## 📱 Responsividade

### Mobile First
- Design começa no celular (até 768px)
- Progressivamente aprimorado para telas maiores

### Breakpoints
```css
/* Celular */
@media (max-width: 768px)

/* Tablet */
@media (min-width: 769px) and (max-width: 1024px)

/* Desktop */
@media (min-width: 1025px) and (max-width: 1279px)

/* TV */
@media (min-width: 1280px)
```

## 🔧 Personalização

### Alterar Breakpoints
Edite o arquivo `estilos/media-query.css`:

```css
/* Exemplo: alterar breakpoint do tablet */
@media screen and (min-width: 800px) and (max-width: 1100px) {
    /* Seus estilos personalizados */
}
```

### Modificar Cores
No arquivo `estilos/style.css`, altere as variáveis CSS:

```css
:root {
    --primary-gradient: linear-gradient(135deg, #sua-cor 0%, #outra-cor 100%);
}
```

## 📊 Informações Técnicas

### Dados Exibidos
- **Largura da tela**: `window.innerWidth`
- **Altura da tela**: `window.innerHeight`
- **Orientação**: Portrait/Landscape
- **DPI**: `window.devicePixelRatio`

### Eventos JavaScript
- `resize`: Atualiza informações em tempo real
- `DOMContentLoaded`: Inicialização
- Media Query Listeners: Detecção de breakpoints

## 🎭 Modos Especiais

### Modo Escuro
Suportado via `prefers-color-scheme: dark`

### Redução de Movimento
Respeita `prefers-reduced-motion: reduce`

### Alta Resolução
Otimização para telas retina com `min-resolution: 2dppx`

## 🖨️ Modo Impressão

Otimização específica para impressão:
- Fundo branco
- Texto preto
- Ocultação de elementos não essenciais
- Layout em coluna única

## 🚀 Próximos Passos

- [ ] Adicionar mais breakpoints
- [ ] Implementar dark mode manual
- [ ] Adicionar gráficos de responsividade
- [ ] Criar versão PWA
- [ ] Adicionar testes automatizados

## 📝 Licença

Este projeto é educacional e pode ser usado livremente para aprendizado de CSS Media Queries.

---

**Desenvolvido com ❤️ para demonstrar o poder das Media Queries**
