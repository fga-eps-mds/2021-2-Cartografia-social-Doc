# <center>Cartografia Social
<p align="justify">
O porjeto Nova Cartografia Social tem o objetivo de promover o mapeamento social comunidades do bioma Amazônia e o fortalecimento da rede de pesquisa envolvida no projeto. O objetivo deste projeto é dar continuidade ao desenvolvimento e implementação de um aplicativo mobile, <a href="https://github.com/fga-eps-mds/2021.1-Cartografia-social-docs">iniciado em 2021.1</a>,  que funcione para auxiliar no mapeamento e registro de situações reais das comunidades, por meio da delimitação de áreas no mapa e marcação de pontos.
</p>

## Membros da equipe
<div class="members">
    <div class="member">
        <p>Rafaella Junqueira
            <!-- <a href="https://github.com/RafaellaJunqueira">Rafaella Junqueira</a> -->
        </p>
        <img src="img/equipe/rafaella.jpeg">
    </div>
    <div class="member">
        <p>Marcos Nery</p>
        <img src="img/equipe/marcos.jpeg">
    </div>
    <div class="member">
        <p>Gustavo Marques</p>
        <img src="img/equipe/gustavoEPS.jpeg">
    </div>
  <div class="member">
    <p>Larissa Sales</p>
    <img src="img/equipe/larissa.jpeg">
  </div>
</div>
  
<div class="members">
    <div class="member">
        <p>Pedro Vitor</p>
        <img src="img/equipe/pedro.jpeg">
    </div>
    <div class="member">
        <p>Eric Chagas</p>
        <img src="img/equipe/eric.jpeg">
    </div>
    <div class="member">
        <p>Gustavo Martins</p>
        <img src="img/equipe/gustavoMDS.jpeg">
    </div>
    <div class="member">
        <p>Vinícius Alves</p>
        <img src="img/equipe/vinicius.jpeg">
    </div>
</div>

<div class="members">
    <div class="one_member">
        <p>Israel Thalles</p>
        <img src="img/equipe/israel.jpeg">
    </div>
    <div class="one_member">
        <p>Gian Medeiros</p>
        <img src="img/equipe/gian.jpeg">
    </div>
    <div class="one_member">
        <p>Gabriel Nascimento</p>
        <img src="img/equipe/gabriel.jpeg">
        <link></link>
    </div>
    <div>
        <img>
    </div>
</div>

<style>
.members {
    display: flex; 
    flex-direction: row;
}
.one_member img {
    position: relative;
    width: 162px;
    opacity: 1;
    border-style: solid;
    border-radius: 640px;
    border-width: 1px; 
    border-color: rgba(0,0,0,0.3);
    z-index: 3;
    transition: opacity 0.5s !important;
}
.one_member p {
    align: center;
    position: absolute;
    transform: translate(0, 2.5em);
    z-index: 2;
    /* color: black; */
    font-weight: bold;
    font-family: Montserrat;
}
.member, .one_member {
    display: flex;
    margin: 5px;
    justify-content: center;
}
.member img {
    position: relative;
    width: 640px;
    opacity: 1;
    border-style: solid;
    border-radius: 640px;
    border-width: 1px; 
    border-color: rgba(0,0,0,0.3);
    z-index: 3;
    transition: opacity 0.5s !important;
}
.member p{
    align: center;
    position: absolute;
    transform: translate(0, 2.5em);
    z-index: 2;
    /* color: black; */
    font-weight: bold;
    font-family: Montserrat;
}
.member img:hover, .one_member img:hover {
    opacity: 0.2;
    z-index: 1;
}
.member p:hover + img, .one_member p:hover + img {
    opacity: 0.3;
    z-index: 1;
}
p {
    font-family: Montserrat !important;
    font-weight: 500;
}
</style>