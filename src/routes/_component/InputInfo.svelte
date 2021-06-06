<script>
  export let title = 'First Name';
  export let req = '';
  export let value= "";
  const onInput = e => (value = e.target.value);
</script>

<style>
    .main {
        width: 180px;
        margin-bottom: 15px;
        margin-right: 20px;
    }

    .box {
        width: 180px;
        height: 40px;
        border: 1px solid var(--text-color);
        background-color: var(--bg-color);
    }

    h1 {
        font-size: 15px;
        font-weight: 300;
        margin-top: 0px;
        margin-bottom: 5px;
    }

    input[type="text"] {
        font-family: 'Montserrat';
        font-size: 30px;
        font-weight: 300;
        color: var(--text-color);
    }

    input:focus {
        outline: 0.5px solid var(--text-color);
    }
</style>
<div class='main'>
    <h1>{title}</h1>

    <input class='box' type={title} name={title} {value} on:input={onInput} {req}/>
</div>
