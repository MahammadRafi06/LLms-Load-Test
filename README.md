﻿# LLM Load Testing Suite

A comprehensive load testing framework for Large Language Models (LLMs) using industry-standard tools and benchmarks.

## Overview

This project provides a unified testing suite for evaluating the performance, scalability, and reliability of LLM deployments under various load conditions. It integrates multiple testing frameworks to provide comprehensive insights into model performance.

## Supported Testing Tools

### **Locust**
- HTTP-based load testing for LLM APIs
- Distributed testing capabilities
- Real-time performance monitoring
- Custom user behavior simulation

### **LLMPerf**
- LLM-specific performance benchmarking
- Token throughput and latency measurements
- Memory usage and resource utilization tracking
- Multi-model comparison capabilities

### **GenAIPerf**
- Generative AI performance testing
- End-to-end latency measurement
- Concurrent request handling
- Response quality assessment

## Features

- **Multi-Framework Support**: Seamlessly switch between different testing tools
- **Configurable Test Scenarios**: Customize load patterns, user behaviors, and test parameters
- **Real-time Monitoring**: Live performance metrics and dashboards
- **Comprehensive Reporting**: Detailed analytics and performance insights
- **Cloud & On-Premise**: Support for various deployment environments
- **Model Agnostic**: Compatible with OpenAI, Anthropic, Hugging Face, and custom models

## Quick Start

### Prerequisites
- Python 3.8+
- pip or conda for package management
- Access to LLM APIs or deployed models

### Installation
```bash
# Clone the repository
git clone https://github.com/your-username/LLms-Load-Test.git
cd LLms-Load-Test

# Install dependencies
pip install -r requirements.txt
```

### Basic Usage
```bash
# Run a simple load test
python run_test.py --tool locust --model gpt-4 --users 10 --duration 5m

# Compare multiple models
python run_test.py --tool llmperf --models gpt-4,claude-3 --benchmark throughput

# Generate comprehensive report
python generate_report.py --test-results results/
```

## Configuration

Test configurations are managed through YAML files in the `config/` directory:
- `locust_config.yaml` - Locust-specific settings
- `llmperf_config.yaml` - LLMPerf benchmarking parameters
- `genaiperf_config.yaml` - GenAIPerf testing configuration
- `models.yaml` - Model endpoints and authentication

## Test Scenarios

- **Stress Testing**: Maximum load capacity determination
- **Spike Testing**: Sudden load increase handling
- **Volume Testing**: Large dataset processing
- **Endurance Testing**: Long-running performance stability
- **Concurrent User Testing**: Multiple user simulation

## Metrics & Reporting

### Performance Metrics
- **Latency**: Response times (p50, p95, p99)
- **Throughput**: Requests per second (RPS)
- **Token Metrics**: Tokens per second, input/output ratios
- **Error Rates**: Failed requests and error types
- **Resource Usage**: CPU, memory, and network utilization

### Report Formats
- HTML dashboards
- JSON/CSV data exports
- Grafana integration
- Custom visualization support

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

- Email: mrafi@uw.edu
- Issues: [GitHub Issues](https://github.com/MahammadRafi06/LLms-Load-Test/issues)
- Documentation: [Wiki](https://github.com/MahammadRafi06/LLms-Load-Test/wiki)

## Roadmap

- [ ] Integration with additional testing frameworks
- [ ] Advanced ML model performance analytics
- [ ] Cloud deployment automation
- [ ] Real-time alerting system
- [ ] Multi-cloud support

---

**Note**: This is a framework for load testing. Please ensure you have proper authorization before testing third-party APIs and respect rate limits and terms of service.
