# Catálogo Online — Jhennyf

Aplicativo Flutter simples que demonstra o padrão arquitetural MVVM (Model–View–ViewModel) usando
`provider` para gerenciamento de estado. O app consome a API pública de produtos Fake Store:

```
https://fakestoreapi.com/products
```

Visão geral
---------
- Tela principal: grade responsiva de produtos (imagem, título, preço).
- Tela de detalhes: imagem ampliada (Hero), título, descrição, categoria e preço.
- Gerenciamento de estado com `Provider` + `ChangeNotifier` (ViewModel).
- Indicação de carregamento e tratamento de erro quando a API não responde.

Principais pastas
-----------------
- `lib/models/` — modelos de domínio (ex.: `product.dart`).
- `lib/services/` — acesso à API (ex.: `api_service.dart`).
- `lib/viewmodels/` — classes que expõem dados e estados para a UI.
- `lib/views/` — telas e widgets (lista e detalhes).

Pré-requisitos
-------------
- Flutter SDK instalado e configurado (versão compatível com o projeto).
- Conexão com a internet para consumir a API Fake Store.

Como rodar (rápido)
-------------------
Abra um terminal na pasta do projeto `catalago_online` e execute:

```bash
# instalar dependências
flutter pub get

# executar no navegador (chrome)
flutter run -d chrome

# ou executar no Windows (se suportado)
flutter run -d windows

# executar no emulador / device Android/iOS
flutter devices
flutter run
```

Testes
------
Há um teste de widget de exemplo. Para rodar os testes:

```bash
flutter test
```

Notas técnicas
--------------
- Arquitetura: MVVM — o `ViewModel` busca os dados via `ApiService` e notifica a UI por `notifyListeners()`.
- O app usa `http` para requisições REST.
- Para evitar rastrear a pasta inteira do Documentos com Git, o projeto está isolado em `Catálogo Online/catalago_online`.

Contribuição
------------
1. Faça um fork do repositório.
2. Crie uma branch com a mudança (`git checkout -b feat/minha-mudanca`).
3. Faça commit das alterações com mensagens claras.
4. Abra um Pull Request.

Licença
-------
Este projeto está disponível sob a licença MIT — sinta-se livre para usar e adaptar.

Contato
-------
Se quiser, abra uma issue no repositório ou me envie uma mensagem no GitHub: `https://github.com/Jhennyf`.

-----
_README atualizado para instruções claras de uso e contribuição._
