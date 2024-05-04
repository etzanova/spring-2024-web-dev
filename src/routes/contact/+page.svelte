<script>
    let formElement
    let firstName = ''
    let lastName = ''
    let email = ''
    let message = ''

function handleSubmit(){
    alert("Form Submitted")
    formElement.reset()
}
</script>
<h1>Contact</h1>
<section class="flow">
<p>Please complete this form for more information. Thank you!

<form on:submit|preventDefault={handleSubmit}>
    <div>
        <label for="first-name">First Name</label>
        <input type="text" id="first-name" name="first-name" 
        bind:value="{firstName}"
        placeholder="Enter first name..." required/>

    </div>

    <div>
        <label for="email">Email</label>
        <input type="email" id="email" name="email"
        bind:value="{email}"
        placeholder="Enter email address..." required/>
        
    </div>

    <div>
        <label for="message">Message</label>
        <textarea name="message" rows="10"
        bind:value="{message}"
        placeholder="Enter message..."required></textarea>
        
    </div>

    <button>Submit</button>
</form>
</section>

<style>
    form {
            max-width: 32rem;
            display:grid;
            gap: 1.5rem;
    }
    
    div{
            display: grid;
            gap: 0.5rem;
    }
    
    input, textarea {
            padding: 0.5rem;
            font-family: inherit;
     }
</style>