# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Jekyll static site, vanilla HTML/CSS/JavaScript, deployed by GitHub Pages. The repository contains the existing build workflow, popular-post generation, asset pipeline, and site checks; no framework migration is part of this product.

## Users

zjc and developers who build or operate event-driven systems on Kafka. They need practical guidance on producers, consumers, partitions, replicas, transactional semantics, KRaft, capacity, reliability, security, migration, monitoring, and troubleshooting.

## Product Purpose

Kafka 零基础实战指南 is a focused reading room for event streaming engineering. It turns a 28-chapter guide into durable, searchable articles. Success means a visitor can move from an architecture decision or production symptom to a concrete command, parameter, diagnostic flow, or reliability checklist.

## Positioning

The site treats Kafka as both an application integration layer and an infrastructure system. Its distinctive path connects message semantics and Spring Boot usage to log storage, replication, controllers, KRaft, performance, operations, and event-driven design.

## Operating Context

Content covers setup, core concepts, command-line practice, producer and consumer internals, topic and partition management, serialization and Schema Registry, Spring Boot integration, log segments and indexes, ISR and high availability, controllers and coordinators, request handling and Purgatory, idempotence, transactions and Exactly Once, rebalance, KRaft, performance testing, capacity planning, reliability practices, monitoring, troubleshooting, security, scaling and migration, Connect, Streams and ksqlDB, log and order-event projects, big-data integration, event-driven patterns, interviews, and a quick-reference appendix. Readers often need commands, configuration, architecture notes, and reliability tables together.

## Capabilities and Constraints

- Preserve existing Jekyll routes and article behavior.
- Preserve primary Chinese navigation labels and article content.
- Keep desktop popular articles and recommended reading.
- Keep search, categories, bookmarks, about, RSS, PWA, and social sharing behavior.
- Keep the GitHub Pages build compatible; avoid a framework or heavy runtime dependency.
- Keep `/kafka` as the stable base path.

## Brand Commitments

Site name is Kafka 零基础实战指南. Default author is zjc. The site language is primarily Chinese. The logo, favicon, and precise event-systems visual language are part of the brand.

## Evidence on Hand

- 29 Markdown articles under `_posts/`, organized by year/month/day.
- Article dates run from 2026-01-01 through 2026-01-29.
- Chapters span fundamentals, client practice, storage and replication, metadata architecture, performance, operations, ecosystem, architecture, interviews, and a quick-reference appendix.
- Existing logo, favicon, search index, RSS, and PWA assets are present.
- No testimonials, customer claims, or commercial metrics are available; none may be invented.

## Product Principles

1. Delivery semantics and operational evidence stay explicit.
2. Commands, configuration, tables, and architecture notes remain first-class content.
3. Client usage and broker internals should feel connected.
4. Reliability checklists support production decisions without replacing judgment.
5. Performance and accessibility constrain every visual decision.
