# Catálogo Online

Aplicativo Flutter demonstrando o padrão MVVM usando Provider para gerenciar estado. O app consome a API pública `https://fakestoreapi.com/products` e mostra uma lista de produtos e uma tela de detalhes.

Funcionalidades:
- Tela principal: lista de produtos (imagem, nome, preço)
- Tela de detalhes: nome, imagem, descrição, preço e categoria
- Indicador de carregamento enquanto busca os dados
- Mensagem de erro com botão de tentativa em caso de falha

Como rodar

1. Tenha o Flutter instalado e configurado na sua máquina.
2. No terminal, vá até a pasta do projeto (onde está `pubspec.yaml`) e execute:

```bash
flutter pub get
flutter run
```

Observações

- O app usa `provider` para state management e `http` para chamadas REST.
- Se preferir, abra o projeto em um IDE (Android Studio / VS Code) e rode a partir dali.
