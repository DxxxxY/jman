<script>
    export const push = (message) => {
        document.querySelector("pre").textContent += `${message}\n`;
    };

    export let title;

    export const clear = () => {
        document.querySelector("pre").textContent = "";
    };
</script>

<div>
    <h1>{title}</h1>
    <pre />
</div>

<style>
    div {
        position: absolute;
        width: 100%;
        height: 100%;
        left: 0;
        top: 0;
        background-color: rgba(20, 20, 20, 0.3);
        backdrop-filter: blur(4px);
        word-wrap: break-word;
    }

    h1,
    pre {
        margin: 0;
        white-space: pre-wrap;
        text-align: left;
    }
</style>
