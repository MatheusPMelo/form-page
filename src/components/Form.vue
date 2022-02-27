<template>
    <div class="container mt-5">
        <div class="col-md-12 d-flex justify-content-center">
            <div class="contentForm  p-2 col-md-6">
                <form @submit.prevent="checkForm" action="#" method="get">
                    <div class="d-flex justify-content-center">
                        <div class="col-md-4 m-2">
                            <input class="p-3" v-model="nome" type="text" name="" id="nome" placeholder="Nome*" required>
                        </div>
                        <div class="col-md-4 m-2">
                            <input class="p-3" v-model="sobrenome" type="text" name="" id="sobrenome" placeholder="Sobrenome*" required>
                        </div>
                    </div>
                    <div class="mt-3 d-flex justify-content-center">
                        <div class="col-md-4 m-2">
                            <input class="p-3" v-model="email" type="email" name="" id="email" placeholder="E-mail*" required>
                        </div>
                        <div class="col-md-4 m-2">
                            <input class="p-3" v-model="senha" type="password" name="" id="senha" placeholder="Senha*" required>
                        </div>
                    </div>
                    <div class="d-flex justify-content-center">
                        <div class="d-flex justify-content-center col-md-9 mt-3">
                            <select class="p-3">
                                <option v-for="opt in opts" :key="opt.id" value="Selecione seu Sexo">{{opt.names}}</option>
                            </select>
                        </div>
                    </div>
                    <div class="d-flex justify-content-center mt-3">
                        <div class="col-md-9 d-flex justify-content-center">
                            <input class="p-2" type="submit" value="Enviar">
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Form',
    data: () => {
        return {
            error: [],
            nome: null,
            sobrenome: null,
            email: null,
            senha: null,

            opts: [
                {names: "Selecione seu sexo"},
                {names: "Feminino"},
                {names: "Masculino"},
                {names: "Não binário"},
            ]
        }
    }    
}
</script>

<style scoped>
input{
    border-radius: .5rem;
    border:none;
    outline: none;
    border: solid 2px #ffffff00;
}
input[type=submit]{
    width: 94%;
    background-color: #2f94ca;
    font-weight: 600;
    color: #fff;
    font-size: 18pt;
    border: solid 3px #2f94ca;
    transition: .5s;
    outline: none;
    border: solid 2px #ffffff00;
}
input:focus, input[type=submit]:focus{
    outline: none;
    border: solid 2px #b394fd;
}
input[type=submit]:hover{
    background-color: #ffffff10;
    border: solid 3px #fff;
    backdrop-filter: blur(2px);
}
select{
    width: 93%;
    border-radius: .5rem;
    border:none;
    outline: none;
    border: solid 2px #ffffff00;
}
select:focus{
    outline: none;
    border: solid 2px #b394fd;
}
</style>