<template lang="">
    <div class="flex-col flex divGlass 2xl:w-9/12 2xl:h-[90%] xl:w-10/12 xl:h-5/6 lg:w-[85%] lg:h-[65%] lg:ml-4 md:w-11/12 md:h-3/4 ml-10 md:ml-0 animate__fadeIn" v-if="enviar"> 
      <h1 class="text-white mt-20 self-center text-3xl tracking-wide font-semibold">Cadastro</h1>  
      <form action="" class="self-center">
        <input type="text" placeholder="Nome" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full" id="nome" v-model="nome">
        <input type="text" placeholder="CPF" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-6/12" id="cpf" v-model="cpf">
        <input type="date" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-2/5 2xl:ml-6 lg:ml-4 md:ml-2" id="date" v-model="data">
        <input type="number" placeholder="Salário" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full" v-model="salario">
        <input name="cep" type="text" placeholder="CEP" id="cep" size="10" maxlength="9" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-2/5" v-model="cep"/>
        <input name="numero" type="text" placeholder="Número" id="numCasa" size="" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] 2xl:ml-6 lg:ml-4 md:ml-2 w-1/4" v-model="numCasa">
        <input name="uf" type="text" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-1/6 2xl:ml-6 lg:ml-4 md:ml-2" placeholder="UF" id="uf" size="2" v-model="uf">
        <input name="rua" type="text" placeholder="Rua" id="street" size="60" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full" v-model="rua">
        <input name="cidade" type="text" id="cidade" size="40" placeholder="Cidade" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-6/12" v-model="cidade">
        <input name="bairro" type="text" id="bairro" size="40" placeholder="Bairro" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-2/5 ml-4 lg:ml-2" v-model="bairro">
        <input type="text" placeholder="Complemento" class="inputCS 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full" id="comp" v-model="comp">
        <button @click="enviar = !enviar" class="btnBase tracking-wide ">Enviar</button>
      </form>
    </div>
    <div class="flex-col flex divGlass 2xl:w-9/12 2xl:h-[90%] xl:w-10/12 xl:h-5/6 lg:w-[85%] lg:h-[65%] lg:ml-4 md:w-11/12 md:h-3/4 ml-10 md:ml-0 animate__fadeIn" v-else>
        <h1 class="text-white mt-20 self-center text-3xl tracking-wide font-semibold">Seus dados:</h1>  
        <div class="self-center divData">
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full" >Nome: {{nome}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-6/12">CPF: {{cpf}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-2/5 2xl:ml-6 lg:ml-4 md:ml-2">Nascimento : {{data}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full" >Salário: {{salario}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-2/5">CEP: {{cep}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] 2xl:ml-6 lg:ml-4 md:ml-2 w-1/4">Número: {{numCasa}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-1/6 2xl:ml-6 lg:ml-4 md:ml-2">UF: {{uf}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full">Rua: {{rua}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-6/12" >Cidade: {{cidade}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-2/5 ml-4 lg:ml-2" >Bairro: {{bairro}}</p>
            <p class="binding 2xl:mt-[7%] xl:mt-[7%] lg:mt-[5%] w-full">Complemento: {{comp}}</p>
        </div>
    </div>
</template>
<script>

export default {
    name: 'BaseForm',
    data() {
        return {
            nome: '',
            cpf: '',
            salario:'',
            data: '',
            cep: '',
            numCasa: '',
            uf:'',
            rua: '',
            cidade:'',
            bairro:'',
            comp:'',
            enviar: true
        }
    },
}

</script>

<style lang="">
    
</style>