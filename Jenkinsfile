#!/usr/bin/env groovy

stage name: 'Build', concurrency: 1
    node {
        // Steps:
        //   - Build Artefact (Image)
        //   - Unit Tests
        //   - Integration Tests
        //   - Contract Tests
        //   - Security Tests
        //   - Metrics
        //   - Publish Artefact
        echo 'Build stage successful'
    }

stage name: 'Acceptance', concurrency: 1
    node {
        // Steps:
        //   - Smoke Tests
        //   - Acceptance Tests
        //   - Functional Tests
        //   - Security Tests
        //   - Load/Stress Tests
        echo 'Acceptance stage successful'
    }

stage name: 'Staging', concurrency: 1
    node {
        // Steps:
        //   - Smoke Tests
        //   - Functional Tests
        //   - Security Tests
        //   - Load/Stress Tests
        //   - Compliance
        echo 'Staging stage successful'
    }

stage name: 'Production', concurrency: 1
    node {
        input message: "Promote to Production?", ok: "Promote"
        // Steps:
        //   - A/B Testing
        //   - Blue / Green Deployment vs. Canary Deployment
        echo 'Successfully released to Production'
    }
