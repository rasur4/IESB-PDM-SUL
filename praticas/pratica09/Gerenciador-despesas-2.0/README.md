# Gerenciador de Despesas 2.0

Aplicativo Expo para registrar, editar, excluir, buscar e acompanhar despesas pessoais com estado global, persistência local, filtros e temas adaptáveis.

## Identificação do aluno

- Nome: Jason Gabriel Alves De Sousa
- Matrícula: 2514290012

## Objetivo

Gerenciar despesas do dia a dia com uma interface simples, acessível e consistente, preservando os dados entre reinicializações do aplicativo e mantendo a experiência funcional em diferentes temas de sistema.

## Funcionalidades implementadas

- Estado global com Context API e reducer imutável
- Persistência local com AsyncStorage na chave `@expenses`
- Cadastro e edição de despesas em uma única tela
- Validação de descrição, valor, data e categoria
- Busca por descrição com debounce e filtros por categoria
- Listas de despesas recentes e todas as despesas
- Resumo com quantidade e total calculados por lista
- Suporte a tema claro e escuro com `useColorScheme`
- Seleção de data com `DateTimePicker`
- Seleção de categoria em modal com animação
- Confirmação de exclusão e retorno ao fluxo anterior

## Tecnologias e dependências

- Expo SDK 57
- React Native 0.86
- React 19
- React Navigation Native Stack e Bottom Tabs
- AsyncStorage
- @expo/vector-icons
- @react-native-community/datetimepicker
- Node.js / npm para instalação e execução

## Requisitos para executar

- Node.js 18+ (recomendado LTS)
- npm
- Expo Go em dispositivo físico ou um emulador Android/iOS
- Git para versionamento local

## Instalação e execução

Na pasta do projeto, execute:

```bash
npm install
npx expo start
```

Para verificar a saúde do projeto:

```bash
npx expo-doctor
npm test
```

## Testes de comportamento

1. Abra o app e adicione uma despesa.
2. Feche e reabra a aplicação para confirmar a persistência via AsyncStorage.
3. Edite uma despesa existente e confirme que os dados são preenchidos automaticamente.
4. Tente salvar com descrição curta, valor zero, data futura ou categoria vazia para verificar as mensagens de erro.
5. Use a busca por descrição para confirmar a filtragem sem diferenciar maiúsculas/minúsculas.
6. Alterna o tema do sistema para validar o contrast e leitura no modo claro e escuro.
7. Exclua uma despesa e confirme a mensagem de confirmação antes da remoção.

## Estrutura do projeto

```text
Gerenciador-despesas-2.0/
├── App.js
├── app.json
├── index.js
├── package.json
├── README.md
├── src/
│   ├── components/
│   │   └── despesa/
│   ├── constants/
│   ├── hooks/
│   ├── screens/
│   ├── store/
│   └── utils/
├── tests/
└── .gitignore
```

## Observações

- O arquivo `.gitignore` já exclui `node_modules` e artefatos do Expo.
- Não há segredos, tokens ou arquivos `.env` armazenados no projeto.
- As capturas de tela do aplicativo devem ser anexadas manualmente ao pull request ou ao relatório final, conforme a prática da disciplina.
