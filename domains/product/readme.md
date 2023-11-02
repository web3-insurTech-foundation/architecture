# Product Domain

The Product Domain relates to products consumers can purchase to cover their assets, loosely, think of an auto insurance policy, which is a product of an insurance company.

# Definitions
The terms used in the Product Domain

## Product
A collection of cover items to be included in a Policy and sets forth the restrictions and limitations.

## Category
A collection is like items from an insurable domain.  For home, some categories are Appliances, Plumbing

## Cover Item 
This is a specific item for cover.  This is sometimes referred to as the Risk. - this is the item that will need replacement.

# General Flow
A Product Manager identifies a need for covered items to be protected, say, microwave ovens.

The Product Manager then evaluates the likelihood of these items failing or requiring the obligation of the Insurer.

This cover item along with the actuarial data forms a Reserve Pool, a set aside pool of money that will be used to reimburse the cover item.

Once underwriting capabilities are put in place, the Product is ready to be marketed.  The Insurance Product Marketplace is where Consumers go to find Product that suit their needs.

The Consumer applies for the Product, is underwritten and the Policy containing the Product is enacted.

# Design Thoughts
- We will have a single Product that will be instantiated many times, as a successful Product will have many subscribers.

- The Product is immutable once created, and therefore a NFT is most appropriate.  The Product NFT is to be included in the Policy NFT - again, another immutable Contract.

- To facilitate new Product delivery and reduce development time, we can centralize the Categories and Cover Items.

- For Risk items, we have replacement value or replace - we need to provide a methodology to allow the Product Manager to appropriately price the Risk items

Refresh for 11/23
