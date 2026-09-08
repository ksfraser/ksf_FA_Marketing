# BR-MKT-001 - Marketing Project Template

## Business Requirement

**Module**: Marketing (new)
**Status**: Proposed

### Marketing Project Template

```
Stage: Strategy & Planning
  - Market Research & Analysis
  - Target Audience Definition
  - Campaign Strategy Development
  - Brand Messaging
  - Budget Planning
  - Timeline Definition

Stage: Creative Development
  - Concept Development
  - Copywriting
  - Design (Print/Digital)
  - Video/Photography Production
  - Brand Guidelines Review
  - Creative Approval

Stage: Campaign Launch
  - Email Campaign Setup
  - Social Media Scheduling
  - Paid Advertising Setup
  - Website Updates
  - PR Distribution
  - Launch Event Planning

Stage: Monitoring & Optimization
  - Performance Tracking
  - A/B Testing
  - Budget Adjustment
  - Content Updates
  - Stakeholder Reporting
  - Campaign Close
```

### Integration

Marketing module owns Opportunities (sales pipeline), Campaigns (project instances), and Contract billing.

Hooks:
```php
hook_invoke_all('marketing_project_template_applied', [
    'template_id' => 'marketing',
    'project_id' => $projectId,
    'stages' => [...],
    'activities' => [...],
]);
```
