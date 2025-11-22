const processLevelData = () => {
  let characterName = '',
    characterXp = 0;


  characterName = prompt('Informe o nome do personagem: ');
  characterXp = Number(prompt('Informe a quantidade de xp do personagem: '));
  let classificacao = '';

  if (characterXp < 1000) {
    classificacao = 'Ferro';
  } else if (characterXp >= 1001 && characterXp <= 2000) {
    classificacao = 'Bronze';
  } else if (characterXp >= 2001 && characterXp <= 5000) {
    classificacao = 'Prata';
  } else if (characterXp >= 5001 && characterXp <= 7000) {
    classificacao = 'Ouro';
  } else if (characterXp >= 7001 && characterXp <= 8000) {
    classificacao = 'Platina';
  } else if (characterXp >= 8001 && characterXp <= 9000) {
    classificacao = 'Ascendente';
  } else if (characterXp >= 9001 && characterXp <= 10000) {
    classificacao = 'Imortal';
  } else if (characterXp >= 10001) {
    classificacao = 'Radiante';
  }

  alert(`O Herói de nome ${characterName} está no nível de ${classificacao}`);
};

processLevelData();
