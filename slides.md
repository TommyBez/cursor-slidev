---
title: Integrating Shadcn CLI and MCP with Cursor
info: |
  Cursor Meetup Florence - Enhancing Development Workflows
class: bg-[#0F0F0F] text-white text-center
mdc: true
theme: slidev-theme-cursor
layout: cover

---

<div class="flex flex-col items-center text-center space-y-8">
  <img src="/assets/Cursor_Italy.png" alt="Cursor Italy" class="w-64 h-64 object-contain" />
  <h1 class="text-5xl font-bold">Welcome to Cursor Italy! 🇮🇹</h1>
  <p class="text-2xl text-blue-300 font-semibold">Florence Meetup</p>
  <p class="text-xl opacity-80">Building the future of AI-powered development together</p>
</div>

---

# Tonight's Journey 🗺️

<div class="space-y-8 text-xl">
  <div class="flex items-center gap-4 p-4 rounded-lg bg-blue-500/20">
    <span class="text-3xl">🔧</span>
    <div>
      <div class="font-bold text-blue-300">Shadcn CLI</div>
      <div class="text-lg opacity-80">Streamlining UI Component Integration</div>
    </div>
  </div>
  
  <div class="flex items-center gap-4 p-4 rounded-lg bg-green-500/20">
    <span class="text-3xl">🔗</span>
    <div>
      <div class="font-bold text-green-300">Model Context Protocol (MCP)</div>
      <div class="text-lg opacity-80">Bridging AI and External Tools</div>
    </div>
  </div>
  
  <div class="flex items-center gap-4 p-4 rounded-lg bg-purple-500/20">
    <span class="text-3xl">🧠</span>
    <div>
      <div class="font-bold text-purple-300">Integration with Cursor</div>
      <div class="text-lg opacity-80">Practical Implementation</div>
    </div>
  </div>
</div>

---

# What is Shadcn/ui? 🎨

<div class="space-y-8">
  <div class="text-center">
    <h2 class="text-4xl font-bold text-blue-300 mb-6">Not a Traditional Component Library</h2>
    <p class="text-xl opacity-90 max-w-4xl mx-auto">
      Shadcn/ui is a <strong class="text-green-300">code distribution platform</strong> and collection of beautifully-designed, accessible components. <strong class="text-yellow-300">This is not a component library. It is how you build your component library.</strong>
    </p>
  </div>
  
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mt-12">
    <div class="space-y-6">
      <h3 class="text-2xl font-bold text-green-300">🔓 Open Code Philosophy</h3>
      <ul class="text-lg space-y-3">
        <li class="flex items-start gap-3">
          <span class="text-green-400 mt-1">✓</span>
          <span>You own the actual component code</span>
        </li>
        <li class="flex items-start gap-3">
          <span class="text-green-400 mt-1">✓</span>
          <span>Full transparency and control</span>
        </li>
        <li class="flex items-start gap-3">
          <span class="text-green-400 mt-1">✓</span>
          <span>No more style overrides or wrappers</span>
        </li>
        <li class="flex items-start gap-3">
          <span class="text-green-400 mt-1">✓</span>
          <span>AI-ready for LLMs to understand</span>
        </li>
      </ul>
    </div>
  </div>
</div>

---

# The Shadcn CLI: Your Code Distribution Tool 🚀

<div class="space-y-8">
  <div class="text-center">
    <h2 class="text-4xl font-bold text-blue-300 mb-4">More Than Just a CLI</h2>
    <p class="text-xl opacity-90 max-w-3xl mx-auto">
      The Shadcn CLI is a <strong class="text-green-300">code distribution system</strong> that copies components directly into your codebase, giving you complete ownership and control.
    </p>
  </div>
  
  
  <div class="bg-gradient-to-r from-blue-500/20 to-green-500/20 rounded-xl p-6 max-w-4xl mx-auto">
    <h3 class="text-2xl font-bold text-yellow-300 mb-4 text-center">Key CLI Features</h3>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <ul class="space-y-2">
        <li class="flex items-center gap-3">
          <span class="text-green-400">✓</span>
          <span>Cross-framework route support</span>
        </li>
        <li class="flex items-center gap-3">
          <span class="text-green-400">✓</span>
          <span>Monorepo support</span>
        </li>
        <li class="flex items-center gap-3">
          <span class="text-green-400">✓</span>
          <span>Custom registry support</span>
        </li>
      </ul>
      <ul class="space-y-2">
        <li class="flex items-center gap-3">
          <span class="text-blue-400">✓</span>
          <span>Tailwind v4 compatibility</span>
        </li>
        <li class="flex items-center gap-3">
          <span class="text-blue-400">✓</span>
          <span>React 19 support</span>
        </li>
        <li class="flex items-center gap-3">
          <span class="text-blue-400">✓</span>
          <span>Component diff tracking</span>
        </li>
      </ul>
    </div>
  </div>
</div>

---

# Why Choose Shadcn/ui? 💪

<div class="text-center space-y-12">
  <h2 class="text-4xl font-bold">The Copy-Paste Revolution</h2>
  
  <div class="bg-gradient-to-r from-yellow-500/20 to-orange-500/20 rounded-xl p-8 max-w-4xl mx-auto">
    <h3 class="text-2xl font-bold text-yellow-300 mb-4">Traditional Libraries vs Shadcn/ui</h3>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 text-left">
      <div>
        <h4 class="text-lg font-semibold text-red-300 mb-2">❌ Traditional Approach</h4>
        <ul class="space-y-1 text-sm opacity-90">
          <li>Install from NPM</li>
          <li>Override styles with workarounds</li>
          <li>Wrap components for customization</li>
          <li>Mix incompatible APIs</li>
          <li>Vendor lock-in</li>
        </ul>
      </div>
      <div>
        <h4 class="text-lg font-semibold text-green-300 mb-2">✅ Shadcn/ui Approach</h4>
        <ul class="space-y-1 text-sm opacity-90">
          <li>Copy code directly</li>
          <li>Edit components as needed</li>
          <li>Consistent, composable API</li>
          <li>Beautiful defaults</li>
          <li>Complete control</li>
        </ul>
      </div>
    </div>
  </div>
</div>

---

<div class="flex flex-col items-center text-center">
  <h1 class="text-6xl font-bold mb-8">🔗 Model Context Protocol</h1>
  <h2 class="text-4xl font-bold text-green-300">Bridging AI and External Tools</h2>
  <div class="text-lg mt-8 opacity-60">The universal connector for AI</div>
</div>

---

# Understanding MCP 🤖

<div class="space-y-8">
  <div class="text-center">
    <h2 class="text-4xl font-bold text-green-300 mb-4">What is MCP?</h2>
    <p class="text-xl opacity-90 max-w-4xl mx-auto">
      The Model Context Protocol (MCP) is an <strong class="text-blue-300">open standard</strong> developed by Anthropic that enables AI applications to connect securely and efficiently with external data sources and tools.
    </p>
  </div>
  
  <div class="bg-gradient-to-r from-blue-500/20 to-green-500/20 rounded-xl p-8 text-center">
    <div class="text-6xl mb-4">🔌</div>
    <h3 class="text-3xl font-bold text-yellow-300 mb-4">Think of MCP as</h3>
    <p class="text-2xl font-semibold">"USB-C for AI Applications"</p>
    <p class="text-lg opacity-80 mt-2">A universal connector for seamless integration</p>
  </div>
</div>

---

# Key Features of MCP ⭐

<div class="grid grid-cols-1 md:grid-cols-3 gap-8 mt-8">
  <div class="bg-white/10 backdrop-blur-sm rounded-xl p-6">
    <div class="text-4xl mb-4 text-center">🔧</div>
    <h3 class="text-xl font-bold text-blue-300 mb-4 text-center">Standardized Integration</h3>
    <p class="text-sm opacity-90">MCP provides a consistent method for AI models to interact with different tools and data sources, eliminating the need for custom integrations.</p>
  </div>
  
  <div class="bg-white/10 backdrop-blur-sm rounded-xl p-6">
    <div class="text-4xl mb-4 text-center">🔒</div>
    <h3 class="text-xl font-bold text-green-300 mb-4 text-center">Secure Communication</h3>
    <p class="text-sm opacity-90">It ensures secure, two-way connections between AI-powered tools and external systems.</p>
  </div>
  
  <div class="bg-white/10 backdrop-blur-sm rounded-xl p-6">
    <div class="text-4xl mb-4 text-center">🔄</div>
    <h3 class="text-xl font-bold text-purple-300 mb-4 text-center">Extensibility</h3>
    <p class="text-sm opacity-90">Developers can build MCP servers to expose their data or tools, and AI applications (MCP clients) can connect to these servers.</p>
  </div>
</div>

---



# Demo Time! 🎬

<div class="text-center space-y-12">
  <h2 class="text-5xl font-bold">Let's See It in Action</h2>
  
  <div class="text-8xl">👨‍💻</div>
  
  <div class="space-y-6">
    <p class="text-2xl text-blue-300 font-semibold">Live Integration Demo</p>
  </div>
</div>
