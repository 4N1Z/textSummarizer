
<script lang = "ts">
    import {initializeApp} from "firebase/app";
    import {getFirestore, setDoc} from "firebase/firestore";
    import {docStore } from "sveltefire";

    const firebaseConfig = {
    };

    const app = initializeApp(firebaseConfig);
    const db = getFirestore();
    const textDoc = docStore<any>(db, "text_document/1");
    
    async function handleSubmit (event:SubmitEvent){
        const data = new FormData(event.target as HTMLFormElement); 
        await setDoc(textDoc.ref!, {
            text:data.get("text"),

        });
    }

</script>

<h1>Text Summariuzer Using PaLM LLM 🌹 </h1>

<h3>User Input</h3>
<form on:submit|preventDefault  ={handleSubmit}>
    <textarea name= "text"/>
    <input type="submit">
</form>
{$textDoc?.text};

<h3> Sumamrized text </h3>
{$textDoc?.summary};