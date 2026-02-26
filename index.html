<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Modo Carreira - Futebol</title>
<style>
body {
    font-family: Arial;
    background: #0f172a;
    color: white;
    text-align: center;
}
button {
    padding: 10px 20px;
    margin: 5px;
    border: none;
    background: #22c55e;
    color: white;
    cursor: pointer;
    font-weight: bold;
}
button:hover {
    background: #16a34a;
}
.card {
    background: #1e293b;
    padding: 10px;
    margin: 10px;
    border-radius: 8px;
}
</style>
</head>
<body>

<h1>⚽ Modo Carreira</h1>
<h2 id="season">Temporada 1</h2>
<h3 id="budget">Orçamento: €5000000</h3>

<button onclick="simulateSeason()">Simular Temporada</button>
<button onclick="nextSeason()">Próxima Temporada</button>

<h2>Elenco</h2>
<div id="squad"></div>

<h2>Tabela</h2>
<div id="table"></div>

<script>
let season = 1;
let budget = 5000000;

class Player {
    constructor(name, age, overall) {
        this.name = name;
        this.age = age;
        this.overall = overall;
        this.potential = overall + Math.floor(Math.random() * 10);
        this.value = overall * 100000;
    }

    develop() {
        if (this.overall < this.potential) {
            this.overall += Math.floor(Math.random() * 2);
            this.value = this.overall * 100000;
        }
        this.age++;
    }
}

class Team {
    constructor(name) {
        this.name = name;
        this.points = 0;
        this.goalsFor = 0;
        this.goalsAgainst = 0;
        this.squad = [];
    }
}

let league = [];
let playerTeam;

function generateLeague() {
    for (let i = 0; i < 6; i++) {
        let team = new Team("Clube " + (i+1));
        for (let j = 0; j < 15; j++) {
            team.squad.push(new Player("Jogador_"+j, rand(18,32), rand(60,85)));
        }
        league.push(team);
    }
    playerTeam = league[0];
}

function simulateMatch(home, away) {
    let homeGoals = rand(0,4);
    let awayGoals = rand(0,4);

    home.goalsFor += homeGoals;
    home.goalsAgainst += awayGoals;

    away.goalsFor += awayGoals;
    away.goalsAgainst += homeGoals;

    if (homeGoals > awayGoals) home.points += 3;
    else if (awayGoals > homeGoals) away.points += 3;
    else {
        home.points += 1;
        away.points += 1;
    }
}

function simulateSeason() {
    for (let i = 0; i < league.length; i++) {
        for (let j = i+1; j < league.length; j++) {
            simulateMatch(league[i], league[j]);
        }
    }

    league.sort((a,b) => b.points - a.points);
    updateTable();
}

function nextSeason() {
    league.forEach(team => {
        team.squad.forEach(player => player.develop());
        team.points = 0;
        team.goalsFor = 0;
        team.goalsAgainst = 0;
    });

    season++;
    budget += 2000000;

    document.getElementById("season").innerText = "Temporada " + season;
    document.getElementById("budget").innerText = "Orçamento: €" + budget;

    updateSquad();
    updateTable();
}

function updateSquad() {
    let squadDiv = document.getElementById("squad");
    squadDiv.innerHTML = "";

    playerTeam.squad.forEach(player => {
        squadDiv.innerHTML += `
            <div class="card">
                <b>${player.name}</b><br>
                Idade: ${player.age} <br>
                Overall: ${player.overall} <br>
                Valor: €${player.value}
            </div>
        `;
    });
}

function updateTable() {
    let tableDiv = document.getElementById("table");
    tableDiv.innerHTML = "";

    league.forEach(team => {
        tableDiv.innerHTML += `
            <div class="card">
                <b>${team.name}</b> - ${team.points} pts
            </div>
        `;
    });
}

function rand(min,max){
    return Math.floor(Math.random()*(max-min+1))+min;
}

generateLeague();
updateSquad();
updateTable();
</script>

</body>
</html>
