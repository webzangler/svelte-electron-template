<script>
  const ipcHandle = () => window.electron.ipcRenderer.send('ping')
</script>

<main class="min-h-screen w-full flex items-center justify-center flex-col gap-4">
  <h1 class="font-bold text-4xl">Electron + Svelte Starter</h1>
  <button class="bg-blue-500 px-4 py-2 rounded-md text-white" on:click={ipcHandle}>Ping</button>
</main>
