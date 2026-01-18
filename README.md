# ⚡ AI Frontend Performance Optimizer

**Powered by OpenAI & Multi-Agent Architecture**

> **Upload performance artifacts, analyze Core Web Vitals, and receive AI-powered optimization recommendations tailored for Next.js 16 and React 19.2—all in a seamless, modern interface.** 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-16-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB.svg)](https://react.dev/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1--mini-green.svg)](https://openai.com/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black.svg)](https://vercel.com/)

---

## ✨ What It Does

AI Frontend Performance Optimizer is an intelligent performance analysis platform that uses a **multi-agent AI workflow** to:

1. **Ingest Performance Data** — Upload Next.js build stats, Lighthouse reports, or PageSpeed Insights JSON
2. **Extract Core Web Vitals** — Parse and normalize LCP, CLS, INP, TTI, and bundle metrics
3. **Generate Recommendations** — Multi-agent AI system produces prioritized, actionable optimization suggestions
4. **Provide Insights** — Interactive dashboard with trends, comparisons, and conversational AI assistance

All optimized for Next.js 16 App Router and React 19.2 patterns.

---

## 🎯 Core Features

### 🤖 **AI-Powered Analysis**
- **Multi-Agent System** — AnalysisAgent, RefactorAgent, and ReviewerAgent work together to refine recommendations
- **OpenAI GPT-4.1-mini Integration** — Intelligent analysis with evidence-based suggestions
- **Customizable Prompts** — Tailor recommendations by priority, category, and focus area
- **Real-time Progress** — Animated progress indicators for long-running analysis jobs

### 📊 **Comprehensive Performance Metrics**
- **Core Web Vitals** — LCP, CLS, INP, TTI tracking and analysis
- **Bundle Analysis** — Identify oversized chunks, duplicate modules, and optimization opportunities
- **Audit Insights** — Lighthouse/PageSpeed opportunities and diagnostics
- **Historical Trends** — Track performance improvements over time with interactive charts

### 🔄 **Comparison & Collaboration**
- **Run Comparison** — Side-by-side comparison of two performance runs with visual diffs
- **Export & Share** — PDF and JSON export options with shareable report links
- **Performance Monitoring** — Set up continuous monitoring with scheduled audits
- **Interactive Playground** — Chat interface to ask questions about your performance data

### 🎨 **Modern UI/UX**
- **Single-Page Architecture** — Smooth state-driven transitions, no page reloads
- **Dark/Light Mode** — Beautiful theme with system preference support
- **Mobile-First Design** — Fully responsive with 44px+ touch targets for optimal mobile experience
- **Real-time Updates** — Live progress tracking with smooth animations

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 📈 **Metrics Dashboard** | Real-time Core Web Vitals tracking with visual indicators |
| 📦 **Bundle Analysis** | Deep dive into bundle composition and optimization opportunities |
| 🔍 **Lighthouse Audits** | Comprehensive audit results with actionable insights |
| 🤖 **AI Recommendations** | Prioritized optimization suggestions with evidence and steps |
| 📊 **Trends Visualization** | Historical performance metrics with interactive charts |
| 🔄 **Run Comparison** | Compare two runs side-by-side with visual diffs |
| 💬 **AI Playground** | Conversational interface for performance questions |
| 📤 **Export/Share** | PDF and JSON export with shareable links |
| ⚙️ **Recommendation Builder** | Customize AI prompts for targeted recommendations |
| 📡 **Live Monitoring** | Scheduled performance monitoring with alerts |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 16.0.10** | React 19.2 with App Router, Server Components, Streaming |
| **TypeScript** | Type-safe development with strict mode |
| **Tailwind CSS** | Utility-first styling with design tokens |
| **shadcn/ui** | Accessible component library built on Radix UI |
| **next-themes** | Seamless dark/light mode with system preference |
| **recharts** | Interactive charts for trends visualization |
| **Lucide Icons** | Modern, consistent icon system |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance async Python API |
| **OpenAI SDK** | GPT-4.1-mini integration with structured outputs |
| **Multi-Agent Architecture** | AnalysisAgent → RefactorAgent → ReviewerAgent pipeline |
| **Pydantic v2** | Runtime type validation and serialization |
| **Uvicorn** | ASGI server for production deployment |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL database with RPC functions for complex queries |
| **Upstash Redis** | Job status caching and PageSpeed API response caching |
| **JSONB Storage** | Efficient artifact storage with query capabilities |

### **External APIs** 🔌
| API | Purpose |
|-----|---------|
| **OpenAI GPT-4.1-mini** | Multi-agent recommendation generation and conversational AI |
| **Google PageSpeed Insights** | Real-world performance metrics (optional) |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting with edge functions |
| **Railway** | Backend API with automatic deployments |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INPUT                               │
│     Upload: Build Stats, Lighthouse, or PageSpeed JSON      │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                 ARTIFACT PARSING & NORMALIZATION            │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │   Next.js    │  │  Lighthouse  │  │  PageSpeed   │      │
│  │ Build Stats  │  │    Report    │  │    Insights  │      │
│  └──────┬───────┘  └──────┬───────┘  └──────┬───────┘      │
│         │                 │                  │               │
│         └─────────────────┼──────────────────┘               │
│                           │                                  │
│                    ┌──────▼───────┐                          │
│                    │   Normalize  │                          │
│                    │  • Metrics   │                          │
│                    │  • Bundles   │                          │
│                    │  • Audits    │                          │
│                    └──────┬───────┘                          │
└───────────────────────────┼──────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────────┐
│              MULTI-AGENT AI RECOMMENDATION PIPELINE         │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │  Analysis    │  │  Refactor    │  │  Reviewer    │      │
│  │   Agent      │──│   Agent      │──│   Agent      │      │
│  │  (Root Cause)│  │ (Solutions)  │  │ (Validation) │      │
│  └──────────────┘  └──────────────┘  └──────┬───────┘      │
└──────────────────────────────────────────────┼───────────────┘
                                               │
                                               ▼
┌─────────────────────────────────────────────────────────────┐
│                       OUTPUT                                │
│  • Prioritized Recommendations (P0/P1/P2)                  │
│  • Evidence-Based Suggestions                               │
│  • Concrete Next.js 16 + React 19.2 Steps                  │
│  • Patch Plans & Expected Impact                            │
│  • Bundle & Audit Insights                                  │
└─────────────────────────────────────────────────────────────┘
```

---

## 📸 Key Highlights

### 🎯 **Performance-First Architecture**
Built with performance in mind—from Core Web Vitals tracking to bundle analysis, every feature helps identify and fix performance bottlenecks.

### 🤖 **Intelligent AI Recommendations**
The multi-agent system doesn't just suggest optimizations—it analyzes root causes, proposes concrete solutions, and validates them for Next.js 16 and React 19.2 best practices.

### 📊 **Data-Driven Insights**
Track performance over time, compare runs, and visualize trends to understand the impact of optimizations.

### 🎨 **Modern Developer Experience**
Smooth animations, real-time updates, and an intuitive interface make performance analysis enjoyable rather than tedious.

---

## 📖 User Guide

### Getting Started

1. **Create a Run** — Navigate to Reports and enter your project details
2. **Upload Artifacts** — Upload Next.js build stats, Lighthouse report, or PageSpeed JSON
3. **Run Analysis** — Choose heuristic or AI-powered analysis
4. **Review Recommendations** — Explore prioritized suggestions with evidence and steps
5. **Track Progress** — Use Trends to visualize improvements over time

### Understanding Core Web Vitals

| Metric | What It Measures | Good Threshold |
|--------|------------------|----------------|
| **LCP** | Largest Contentful Paint | < 2.5s |
| **CLS** | Cumulative Layout Shift | < 0.1 |
| **INP** | Interaction to Next Paint | < 200ms |
| **TTI** | Time to Interactive | < 3.8s |

### Pro Tips

- **Combine Artifacts** — Upload both build stats and Lighthouse for comprehensive analysis
- **Use Trends** — Track performance improvements across multiple runs
- **Customize Recommendations** — Use the Recommendation Builder to focus on specific areas
- **Compare Runs** — Use the comparison feature to see before/after improvements
- **Ask Questions** — Use the Playground to get specific answers about your performance data

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Analysis Time | ~20-30 seconds (AI) |
| Frontend Bundle | Optimized with Next.js 16 |
| Lighthouse Score | 90+ |
| Mobile Ready | ✅ Yes (44px+ touch targets) |
| Core Web Vitals | Optimized (LCP, CLS, INP) |

---

## 🛡️ Security & Privacy

- ✅ Artifact data stored securely in Supabase
- ✅ API rate limiting for external API calls
- ✅ CORS protection for API endpoints
- ✅ Environment variables for all secrets
- ✅ Input validation and sanitization
- ✅ No automatic code modifications (recommendations only)

---

## 👨‍💻 Creator

**Derril Filemon**

This project demonstrates expertise in:

- 🤖 **AI/ML Integration** — Multi-agent systems, OpenAI SDK, structured outputs
- ⚛️ **Modern React** — Next.js 16, React 19.2, Server Components, App Router
- 📊 **Performance Optimization** — Core Web Vitals, bundle analysis, optimization strategies
- 🐍 **Python Backend** — FastAPI, async/await, type-safe APIs
- 🎨 **UI/UX Design** — Responsive design, accessibility, smooth animations
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔧 **DevOps** — CI/CD, environment management, monitoring

---

## 🙏 Acknowledgments

- **[OpenAI](https://openai.com/)** — GPT-4.1-mini API for intelligent analysis
- **[Supabase](https://supabase.com/)** — PostgreSQL database and RPC functions
- **[Upstash](https://upstash.com/)** — Redis caching for job status and API responses
- **[Railway](https://railway.app/)** — Backend deployment platform
- **[Vercel](https://vercel.com/)** — Frontend hosting with edge functions
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful, accessible component library
- **[Google PageSpeed Insights](https://pagespeed.web.dev/)** — Performance metrics API

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
