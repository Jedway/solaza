<section id="how-it-works" class="py-20 bg-black-50">
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12">How It Works</h2>
    <div class="max-w-4xl mx-auto">
      <div class="grid gap-8">
        {#each steps as step, i}
          <div class="flex gap-6 items-start">
            <div class="w-12 h-12 rounded-full bg-blue-600 text-white flex items-center justify-center flex-shrink-0">
              {i + 1}
            </div>
            <div>
              <h3 class="text-xl font-bold mb-2">{step.title}</h3>
              <p class="text-gray-600">{step.description}</p>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>

<script>
  const steps = [
    {
      title: "Create Your Account",
      description: "Sign up in minutes with our simple verification process."
    },
    {
      title: "Connect Your Wallet",
      description: "Link your preferred cryptocurrency wallet or bank account."
    },
    {
      title: "Start Trading",
      description: "Execute secure international transactions with minimal fees."
    }
  ];
</script>