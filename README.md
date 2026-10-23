# Gerenciador de Despesas 2.0

## Identificação do aluno
- Nome: Jason Gabriel Alves De Sousa
- Matrícula: 2514290012

## Objetivo
Aplicativo Expo para registrar, editar, excluir, buscar e acompanhar despesas pessoais com estado global, persistência local e temas adaptáveis.

## Funcionalidades implementadas
- Estado global com Context API e reducer imutável
- Persistência local com AsyncStorage
- Cadastro, edição e exclusão de despesas
- Validação de descrição, valor, data e categoria
- Busca por descrição com debounce e filtro por categoria
- Listas de despesas recentes e gerais
- Resumo com quantidade e total
- Suporte a tema claro e escuro
- Seleção de categoria em modal e data com DateTimePicker

## Tecnologias
- Expo
- React Native
- React Navigation
- AsyncStorage
- @expo/vector-icons
- @react-native-community/datetimepicker

## Testes realizados
- npx expo-doctor
- npm test -- --test-reporter=spec

## Capturas de tela
- [ ] Modo claro
- [ ] Modo escuro
- [ ] Formulário com validações
