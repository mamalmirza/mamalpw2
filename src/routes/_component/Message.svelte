<script>
  export let text = 'Message';
  export let req = '';

  export let value = "";
  const onInput = e => (value = e.target.value);

</script>

<style>
    .main {
        width: 250px;
        margin-bottom: 15px;
        margin-right: -10px;
    }

    .box {
        width: 250px;
        height: 120px;
        border: 1px solid var(--text-color);
        background-color: var(--bg-color);
    }

    h1 {
        font-size: 15px;
        font-weight: 300;
        margin-top: 0px;
        margin-bottom: 5px;
    }

    textarea[type="text"] {
        font-family: 'Montserrat';
        font-size: 30px;
        font-weight: 300;
        color: var(--text-color);

    }

    textarea:focus {
        outline: 0.5px solid var(--text-color);
    }

    textarea {
        resize: none;
    }
</style>
<div class='main'>
    <h1>{text}</h1>

    <textarea class='box' type={text} cols="40" rows="5" name=message {value} on:input={onInput} {req}/>

</div>
