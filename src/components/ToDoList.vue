<template>
    <div>
    <div class="boards">
        <div class="boardquadro">
            <div class="title">
                <div class="board_quadro">
                    <h3>Em Aberto</h3>
                    <div class="button">
                        <button id="new_activ">+</button>
                    </div>
                </div>
            </div>
            <div class="drop">
                <div class="dropzone">
                    <div class="card" draggable="true">
                        <div class ="status blue"></div>
                        <div class="content" >1293</div>
                        <div class="timer_container">
                            <div class="timerDisplay">
                                00 : 00 : 00
                            </div>
                            <div class="buttons">
                                <button id="startTimer">Iniciar</button>
                                <button id="pauseTimer">Pausar</button>
                                <button id="resetTimer">Resetar</button>
                            </div>
                        </div> 
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="boards">
        <div class="board">
            <h3>Fazendo</h3>
            <div class="dropzone">
                <div class="card" draggable="true">
                    <div class ="status yellow"></div>
                    <div class="content"  >1238</div>
                        <div class="timer_container">
                            <div class="timerDisplay">
                                00 : 00 : 00
                            </div>
                            <div class="buttons">
                                <button id="startTimer">Iniciar</button>
                                <button id="pauseTimer">Pausar</button>
                                <button id="resetTimer">Resetar</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="boards">
        <div class="board">
            <h3>Atrasadas</h3>
            <div class="dropzone">
                <div class="card" draggable="true">
                    <div class ="status red"></div>
                    <div class="content"  >1235</div>
                        <div class="timer_container">
                            <div class="timerDisplay">
                                00 : 00 : 00
                            </div>
                            <div class="buttons">
                                <button id="startTimer"> Iniciar</button>
                                <button id="pauseTimer">Pausar</button>
                                <button id="resetTimer">Resetar</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    <div class="boards">
        <div class="board">
            <h3>Finalizadas</h3>
            <div class="dropzone">
                <div class="card" draggable="true">
                    <div class ="status green"></div>
                    <div class="content" >1234</div>
                        <div class="timer_container">
                            <div class="timerDisplay">
                                00 : 00 : 00
                            </div>
                            <div class="buttons">
                                <button id="startTimer">Iniciar</button>
                                <button id="pauseTimer">Pausar</button>
                                <button id="resetTimer">Resetar</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name:"ToDolist"        
    }
</script>

<style scoped>


    /* body {
        background: #130f0d ;
        color: white;
    } */

    .boards {
        display:block;
        flex-direction:column;
        justify-content: space-between;
        width: 100%;
    }

    .boardquadro {
        background:#271d18;
        color: #fd951fcc;
        border: 1px solid #fd951f11;
        border-radius: 6px;
        margin: 0 16px;
        display:flex;
        flex-direction: column;
        /* justify-content:space-between; */
        width: 80%;
    }

    .board {
        background:#271d18;
        border: 1px solid #fd951f11;
        border-radius: 4px;
        margin: 0 16px;
        display: flex;
        flex-direction: column;
        /* justify-content: space-between; */
        width: 100%;
    }
    


    .board h3 {
        padding: 16px ;
        margin: 0;
        color: #fd951fcc;
    }


    .button {
        color: #ffffff;
        width: 45%;
        margin: 5px auto 5px auto;
        display: flex;
        justify-content:space-between;
        /* padding: 12px 15px;  */
        cursor: pointer;
    }
    .dropzone {
        padding: 16px;
        min-height: 300px;
        min-height: 200px;
    }

    .drop{
        display:flex;
        justify-content: space-between;
    }

    .card {
        padding: 16px;
        box-shadow:  2px 2px -1px #fd951fcc;
        width: 350px;
        height: 250px;
        margin: 25px 0;
        border-radius: 4px;
        font-weight:600px;
        font-size:18px;
        background-color:#1a1a1c;
    }

    .status{
        width: 25px;
        height: 10px;
        margin-bottom: 14px;
        border-radius: 8px;
        background: white;
    } 

    .status.blue {
        background:#33adff;
    }

    .status.red {
        background:red;
    }

    .status.green {
        background:#23d2ac
        ;
    }
    .status.yellow {
        background:yellow;
    } 

    .highlight {
        background-color: #ccc;
    }

    .card, .dropzone{
        transition: 400ms;
    }

    .is-dragging{
        cursor: move;
        opacity: 0.3;
    }

    .over{
        background-color: #4cd13711;
    }



</style>