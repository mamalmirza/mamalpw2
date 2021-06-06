<script>
  import BigButton from '../_component/BigButton.svelte';
  import InputInfo from '../_component/InputInfo.svelte';
  import Message from '../_component/Message.svelte';

  let firstName;
  let lastName;
  let subject;
  let email;
  let message;

  let result = {
    txt: '',
    status: 'INIT'
  };

  function submit() {
    if (!email || result.status === 'LOADING') {
      return
    }

    result = {
      status: 'LOADING',
      txt: 'Sending your message ...'
    }

    fetch('https://mamal-pw2-backend.mirzaei-mohammadreza1997.workers.dev/', {
      method: 'POST',
      headers: {
        'content-type': 'application/json'
      },
      body: JSON.stringify({firstName, lastName, email, subject, message})
    }).then(async (res) => {
      if (res.status === 200) {
        const ans = await res.json();
        result = {
          status: 'SUCCESS',
          txt: ans.msg
        }
        console.log(ans);
      }
    }).catch(() => {
      result = {
        status: 'FAIL',
        txt: 'Error occurred while sending message.'
      }
    })
  }
</script>

<style>
    .page {
        flex-direction: column;
        align-items: center;
        display: flex;

    }

    .main {

        width: 953px;
        height: 300px;

        margin-top: 25px;
        margin-bottom: 25px;
        background-color: transparent;
        display: flex;
        flex-direction: row;
        align-items: top;
        justify-content: space-between;

    }

    .row1 {

        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }

    .row {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }

    .title {
        margin-top: 0px;
        margin-bottom: 5px;
        font-size: 15px;
        font-weight: 700;
        padding: 0px;


    }

    .detail {
        font-size: 12px;
        font-weight: 300;
        margin: 0px;
        padding: 0px;
    }

    .bigtitle {
        margin-bottom: 5px;
        margin-top: 0px;
        font-size: 35px;
        font-weight: 700;
    }

    .l1 {
        padding-bottom: 30px;
    }

    .l2 {
        padding-bottom: 15px;
    }

    .circle {
        width: 120px;
        height: 120px;
        padding-right: 15px;
        padding-top: 15px;
    }

    .result-box {
        width: 100%;
        text-align: center;
        margin: 10px 0;
        padding: 20px;
        border: 1px solid gray;
    }

    .green-border {
        border-color: green;
    }

    .red-border {
        border-color: red;
    }

</style>


<div class='page'>
    <div class='main'>
        <div class='left'>
            <div class='l1'>
                <h1 class='bigtitle'>Contact</h1>
                <h2 class='detail'> Looking forward hearing from you</h2>
            </div>
            <div class='l2'>
                <h1 class='title'> Phone </h1>
                <h2 class='detail'> +989333406081 </h2>
            </div>

            <div>
                <h1 class='title'> Email </h1>
                <h2 class='detail'> mirzaei.mohammadreza1977@gmail.com </h2>
            </div>
        </div>
        <div class='right'>
            <div class='row'>
                <InputInfo title='First Name' bind:value={firstName}/>
                <InputInfo title='Last Name' bind:value={lastName}/>
            </div>
            <div class='row'>
                <InputInfo title='Email*' bind:value={email} req='required'/>
                <InputInfo title='Subject' bind:value={subject}/>
            </div>

            <div class='row1'>
                <Message bind:value={message}/>
                <div class='circle'>
                    <BigButton title='Submit' on:submit={submit}/>
                </div>
            </div>

            {#if (result.status !== 'INIT')}

                <div class="result-box"
                     class:green-border={result.status === 'SUCCESS'}
                     class:red-border={result.status === 'FAIL'}>
                    {result?.txt}
                </div>
            {/if}

        </div>
    </div>
</div>
