<section id="features" class="py-20 bg-gray-800">
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12 text-gray-100">Why Choose Solaza</h2>
    <div class="grid md:grid-cols-3 gap-8">
      {#each features as feature}
        <div class="p-6 rounded-xl bg-gray-900 border border-gray-700 hover:shadow-xl hover:shadow-blue-500/10 transition-all duration-300 hover:-translate-y-1">
          <div class="text-2xl mb-4">{feature.icon}</div>
          <h3 class="text-xl font-bold mb-2 text-gray-100">{feature.title}</h3>
          <p class="text-gray-400">{feature.description}</p>
        </div>
      {/each}
    </div>
  </div>
</section>

<script>
  const features = [
    {
      icon: "🔒",
      title: "Secure Transactions",
      description: "Enterprise-grade security with advanced encryption and blockchain verification."
    },
    {
      icon: "⚡",
      title: "Lightning Fast",
      description: "Complete international transfers in minutes, not days."
    },
    {
      icon: "💰",
      title: "Low Fees",
      description: "Save up to 90% on transaction fees compared to traditional banks."
    }
  ];
</script>