# 👋 Hi, I'm Junyeong Kim

> *I read C source for fun. Sometimes I send patches back.*

<p align="left">
  <img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black" />
  <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/eBPF-FF6B35?style=flat-square&logo=linuxfoundation&logoColor=white" />
  <img src="https://img.shields.io/badge/GDB-A42E2B?style=flat-square&logo=gnu&logoColor=white" />
</p>

---

## 🧑‍💻 About

- 🎓 3rd-year CS student at **Jeonju University**
- 🐧 Drawn to **systems programming** — kernels, tracers, runtimes
- 🌱 Active in open source: `uftrace` · `valkey` · `stumpless` · `airflow`
- 🛠️ Currently building **VectorGuard** (eBPF runtime security) & **VectorWave** (LLM framework)
- 💬 Korean / English

---

## 🚀 Featured Projects

### 🛡️ [VectorGuard](https://github.com/Cozymori/VectorGuard)
> **eBPF-based Linux runtime security daemon.** Monitors syscalls in real time and kills threats at the kernel level — no userspace round-trip.

- **Fast Path** — TOML rule engine, hot-reload in <500ms, kernel-level block via `bpf_send_signal(SIGKILL)`
- **Slow Path** — Behavior embedding → Qdrant similarity search to flag unknown attack patterns
- **Adapters** — Native eBPF tracepoints + LSM hooks, with Tetragon / Falco / auditd integrations
- **Deploy** — Docker Compose · systemd · Kubernetes DaemonSet (Helm)

`Rust` · `eBPF` · `LSM` · `Aya` · `Qdrant` · `Kubernetes`

---

### 🌊 [VectorWave](https://github.com/Cozymori/VectorWave)
> A decorator-based framework that turns LLM apps into **self-optimizing, self-healing systems**.

Capture function execution context, serve semantically similar inputs from a vector cache, and let an autonomous agent open PRs that fix runtime errors.

```python
@vectorize(semantic_cache=True, cache_threshold=0.95)
def expensive_llm_task(query: str):
    ...
```

`Python` · `Rust (PyO3)` · `Weaviate` · `HNSW` · `LLM`
**⭐ 22 · 19 releases · MIT**

---

### 🔌 [TransparentClass](https://plugins.jetbrains.com/plugin/28542-transparentclass)
> **IntelliJ IDEA plugin** — published on JetBrains Marketplace.

Surfaces non-private inherited fields and methods from the superclass directly inside the child class editor, so you can see the full shape of a class without jumping between files.

`Kotlin` · `IntelliJ Platform SDK` · `PSI`

---

## 🌱 Open Source Contributions

### ⭐ [uftrace](https://github.com/namhyung/uftrace)
- `feat` Add `cpu` field for per-function CPU execution info — [#2039](https://github.com/namhyung/uftrace/pull/2039) ✅
- `feat` Graph fields (total/self avg, min, max) in `cmds` & `tui` — [#1999](https://github.com/namhyung/uftrace/pull/1999) ✅
- `feat` Support min/max timestamp in `uftrace report` — [#2032](https://github.com/namhyung/uftrace/pull/2032) ✅

<details>
<summary><i>+6 more merged PRs (tests, build, fixes)</i></summary>

- `test` Filter `system_initialize_function` in t295 & t296 — [#2001](https://github.com/namhyung/uftrace/pull/2001) ✅
- `build` Enhance shell script install for Rocky Linux 9 — [#2002](https://github.com/namhyung/uftrace/pull/2002) ✅
- `fix` Build error in `elf_for_each_comment()` — [#2034](https://github.com/namhyung/uftrace/pull/2034) ✅
- `fix` Fix `htmlLabels` config value to boolean `true` — [#2036](https://github.com/namhyung/uftrace/pull/2036) ✅
- `fix` Compiler warnings in `demangle` & `session` — [#2042](https://github.com/namhyung/uftrace/pull/2042) ✅
- `test` Fix exit code of `nightly check_commits step` - [#2046](https://github.com/namhyung/uftrace/pull/2046) ✅

</details>

### ⭐ [airflow](https://github.com/apache/airflow) 
- `feat` Task SDK: Add `Variable.keys()` to list variable keys by prefix — [#66022](https://github.com/apache/airflow/pull/66022) ✅
- `i18n` Korean translation — [#66267](https://github.com/apache/airflow/pull/66267) ✅

### ⭐ [valkey](https://github.com/valkey-io/valkey)
- `test` Migrate cluster tests to new framework, remove legacy files — [#3382](https://github.com/valkey-io/valkey/pull/3382) ✅

### ⭐ [stumpless](https://github.com/goatshriek/stumpless)
- `feat` Implemented `struct to_string` — [#501](https://github.com/goatshriek/stumpless/pull/501) ✅
- `i18n` Korean translation — [#502](https://github.com/goatshriek/stumpless/pull/502) ✅



---

📧 [junyeonggim5@gmail.com](mailto:junyeonggim5@gmail.com)
