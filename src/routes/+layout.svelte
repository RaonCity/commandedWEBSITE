<script>
    const page_name = "Gagaball downloader"
</script>

<h1>{page_name}</h1>
<form>
    <p>이동할 페이지(Slug)의 이름이 입력한 후 이동 버튼을 눌러주십시오.</p>
    <input type="text" id="page_id"><button on:click={() => {
        const page_id = document.getElementById("page_id").value
        location.href = `/${page_id}`}}>이동</button>
</form>

<slot></slot>