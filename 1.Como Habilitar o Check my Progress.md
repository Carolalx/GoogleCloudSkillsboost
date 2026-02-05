# Como Habilitar o Check my Progress - lateral

- Entre em um LAB,  adicione a página como atalho (`CTRL` + `D`), salve;
- Clique no atalho com o botão direito do mouse e selecione `Editar`;
- Escolha o nome que quiser tipo `scores`; e em URL cole o código:

```bash
javascript:(function () {
    const removeLearboard = document.querySelector('.js-lab-leaderboard');
    const showScore = document.querySelector('.games-labs');

    removeLearboard.remove();
    showScore.className = "lab-show l-full no-nav application-new lab-show l-full no-nav "
})();
```

- Quando estiver em um LAB e quiser ativar a contagem, clique no atalho.
